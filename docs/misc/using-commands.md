commands are a way to send messages between clients and the server.
in this case you want to notify the client whenever it should display a killstreak message which is determined by
- the player who just did the killstreak
- the number of kills they did

there are (basically) two places where you can use commands: `CBlob` and `CRules`.
usually you use `CBlob` commands when you want to pass data around specific to a blob, e.g. the "placeBlock" command for builders is sent by clients to tell the server that a block placement was requested by a given blob.
the rest of the time you use `CRules` commands.

in this case you probably want a rules command.

in order to be able to use a command, you first need to register it both on the client and the server.
you would create a rules script, and you would do:
```angelscript
void onInit(CRules@ rules)
{
    rules.addCommandID("killstreak message");
}
```

commands can contain arbitrary data (usually called a payload in networking), which is packed using a `CBitStream`. first we should consider how we want the data to be represented. in this case we will be serializing (= writing) the killstreak player netid (u16) and kill count (u16 will be fine). this is done using the `.write_*` methods.

there are several `SendCommand` methods to `CRules`, in this case we want to use the `SendCommand(uint8 cmd, CBitStream&in params)` one. as we will be using it from the server, it will broadcast the command to all clients.
it requires knowing the command ID that was registered earlier on in `onInit`, which we can query using `getCommandID`.

so effectively the command sending process would look like this:

```angelscript
CBitStream bs;
bs.write_u16(player_netid);
bs.write_u16(kill_count);
rules.SendCommand(rules.getCommandID("killstreak message"), bs);
```

then you need to use the `onCommand` hook to be able to receive the command (sent by the server in this case).
you will want to deserialize (= read) the data, closely matching the write order and types. this is done using `saferead_*` methods. those take an `&out` reference (a reference to the variable that the function can write into), and return a bool that return whether reading succeeded.
`read_*` methods exist but they do not do sanity checking so those are garbage.

```angelscript
void onCommand(CRules@ rules, u8 cmd, CBitStream @params)
{
    // we only do client-side processing in this case anyway
    if (isClient())
    {
        // is the command actually intended for our script?
        if (cmd == rules.getCommandID("killstreak message"))
        {
            u16 player_netid, kill_count;

            // those are evaluated in order
            if (!saferead_u16(player_netid)
             || !saferead_u16(kill_count))
            {
                print("failed to parse killstreak message payload");
                return;
            }

            client_AddToChat(...);
        }
    }
}
```
