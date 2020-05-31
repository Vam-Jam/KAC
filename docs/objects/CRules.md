# CRules@ class
Rules of the game. Think CBlob but it survives the next map purge.

+ Scripts that use CRules usually need to be specified in gamemode.cfg
+ The order in which what functions such as onInit are called are dependant on what order they are in gamemode.cfg
---

## void onInit( CRules@ this )
For the server, this happens once when the server starts <br>
For the client, this happens when they join. <br>
<br>