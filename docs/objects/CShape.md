# CShape@ class
The class used for collisions.

Something you use and get from CBlob

---

## CShape@ getShape()
Returns the shape. Can be used on any blob. Can return null.
<details>
<summary>Example</summary>

```as
CShape@ shape = blob.getShape();
if (shape !is null) // make sure we dont run into a null error
{
    shape.SetStatic(true); // change what we want
}
```

</details>