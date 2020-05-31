# CBlob@ class

---

## void Init()
This calls all current scripts attached to the blob ``onInit(CBlob@ this)`` hook.
<br>
It's commonly used after using ``server_CreateBlobNoInit(const string&in)``, so attributes can be set before onInit is called
<br>
<br>
<small>Returns: void</small>

#### Example: 
```
CBlob@ new_blob = server_CreateBlobNoInit("new_blob"); // new blob
if (new_blob !is null)
{
    new_blob.Tag("very-cool-tag"); // set some important tag/info
    new_blob.Init(); // tell the blob to Init all scripts
}
```
<br>
<br>

## float getHealth()
This returns an f32 in the amount of HP the blob currently has.
<br>
<br>
<small>Returns: f32 - current health</small>

#### Note:
Health returned is current hp / 2.
<br>
Example: If you have 3 hearts, the returned value is ``1.5f``

#### Example: 
```
f32 currentHp = this.getHealth(); // store our current HP for later
```
<br>
<br>

## float getInitialHealth()
This returns an f32 with the amount of HP stated in our blobs .cfg file.
<br>
<br>
<small>Returns: f32 - with starting hp</small>

#### Note:
Health returned is current hp / 2.
<br>
Example: If you have 3 hearts, the returned value is ``1.5f``

#### Example: 
```
f32 hpOnStart = this.getInitialHealth();
```
<br>
<br>
