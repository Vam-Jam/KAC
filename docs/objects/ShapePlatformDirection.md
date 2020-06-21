# ShapePlatformDirection class
Used to define a blob as a platform. The platform doesn't have a position relative to the blob. It's just angle from which the blob will or wont collide.
You can add a platform to a blob by setting `shape_platform = yes` in the config (not recommend) or by using `CShape::AddPlatformDirection`.

`shape_platform = yes` Is the equivalent of calling `CShape::AddPlatformDirection(Vec2f(0, -1), 45, true)`.

Collision with a platform happens if the normal of the collision with the platform direction creates and angle less than the limit, and if the overlap with the object is less than 20% of the objects area.

### Example of how to check platform direction for a call to CMap::HitInfosFromRay
```c
...
CBlob@ b = hits[i].blob;
if (blob !is null && blob.isPlatform())
{
    ShapePlatformDirection@ platform = blob.getShape().getPlatformDirection(0);
    // rotate platform direction
    Vec2f platformDirection = platform.direction;
    if (!platform.ignore_rotations)
    {
        platformDirection.RotateBy(b.getAngleDegrees());
    }

    if (Maths::Abs(platformDirection.AngleWith(rayDirection)) < platform.angleLimit)
    {
        print("the ray collided with a platform!");
    }

}
```

The above code is almost exactly what the engine does internally for collisions except with the collision normal.

## Vec2f directions
The direction of the platform. This should be a normalized vector. Vec2f(0, -1) is up.

## float angleLimit
The angle with relative to the platform direction that collisions are allowed. You usually want to set this to 89 degrees.

## bool ignore_rotations
Whether the rotation of the blob should be taken into account for the platform direction.
