# CMap@ class
Contains useful functions and data about the map in which the blobs interact with.

---

## CMap@ getMap()
Returns the map. Can be used anywhere
#### Example:
```
CMap@ map = getMap();
printFloat(map.tilesize);
```

## bool rayCastSolid(Vec2f startPosWorldspace, Vec2f endPosWorldspace, Vec2f&out pointPosWorldspace)
Casts a ray from `startPosWorldspace` to `endPosWorldspace`. `pointPosWorldspace` is set to the postion the ray is stopped or the `endPosWorldspace` if the ray is not stopped.
<br>
The raycast is stopped if a tile inside the ray is solid or if the blob associated with the tile is collidable.

<small>Returns: true if the rayCast is stopped before `endPosWorldspace`</small>

#### Example:
```
CMap@ map = getMap();

Vec2f pos = this.getPosition();
Vec2f endPos = pos + Vec2f(32, 0);
Vec2f result;

if (!map.rayCastSolid(pos, endPos, result))
{
    print("ray cast didn't hit anything!");

}
else
{
    print("ray cast stopped at: " + result);
}
```

## bool rayCastSolid(Vec2f startPosWorldspace, Vec2f endPosWorldspace)
The same as rayCastSolid.

## bool rayCastSolidNoBlobs(Vec2f startPosWorldspace, Vec2f endPosWorldspace, Vec2f&out pointPosWorldspace)
The same as `rayCastSolid` except it ignores blobs associated with the tile.

## bool rayCastSolidNoBlobs(Vec2f startPosWorldspace, Vec2f endPosWorldspace)
The same as rayCastSolidNoBlobs.

## bool getHitInfosFromArc(Vec2f originPosWorldspace, float angleDegrees, float arcDegrees, float distance, CBlob@ hitter, bool raycast_blobs, HitInfo@[]@ list)
Returns all blobs and tiles with in the arc created.
<br>
`originPosWorldspace` is the origin of the circle the arc is on.
<br>
`angleDegrees` is the start angle of the arc.
<br>
`arcDegrees` is the number of degrees from the start of the arc to the end of the arc.
<br>
`distance` is the radius of the circle the arc is on.
<br>
`hitter` is a blob to be filtered out of the retrieved list.
<br>
`raycast_blobs` whether the arc should check for blobs to be added to the list.
<br>
`list` a HitInfos array to be filled with data about hits.

For each blob in the arc it will check `raycastSolidNoBlobs` to check if they can be reached. If the raycast fails the blob is not added to the list.

<small>Returns: true if list.length > 0</small>

## Example
```
CMap@ map = getMap();

Vec2f pos = this.getPosition();

HitInfo@[] hits;
if( map.getHitInfosFromArch(pos, -45, 45, 36.0f, this, true, hits))
{
    for (int i = 0; i < hits.size(); i++)
    {
        CBlob@ b = hits[i].blob;
        if (b !is null)
        {
            this.server_Hit(b, b.getPosition(), Vec2f_zero, 1.0f, 0);
        }

    }
}
```

## bool getHitInfosFromArc(Vec2f originPosWorldspace, float angleDegrees, float arcDegrees, float distance, CBlob@ hitter, HitInfo@[]@ list)
Calls getHitInfosFromArc with raycast_blobs set to true.

## bool getHitInfosFromRay(Vec2f originPosWorldspace, float angleDegrees, float distance, CBlob@ hitter, HitInfo@[]@ list)
Calls `getHitInfosFromArc` with an `arcDegrees` of 0 and raycast_blobs set to true.

## bool getHitInfosFromCircle(Vec2f originPosWorldspace, float radius, CBlob@ hitter, HitInfo@[]@ list)
Calls `getHitInfosFromArc` with an `arcDegrees` of 360 and raycast_blobs set to true.
