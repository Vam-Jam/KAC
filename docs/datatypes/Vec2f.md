# Vec2f class

Vec2f (also known as Vector2d in other engines) is a class that simply holds an X value, and a Y value. It's used extremely often in KAG.

---

# Properties
Gives you read and write access to any variable below.

### float x

### float y


---

# Constructors
Initiates the class 

### \<constructor>\()
This will return a Vec2f with both x and y as 0

### \<constructor>\( float x, float y )
This will return a Vec2f with the values you pass inside the constructor


# Operators

### Vec2f& opAssign( const Vec2f&in )
This will allow you to assign a new value to the current Vec2f using the = operator

### Vec2f opMul( float value ) 
This will multiply the current Vec2f x and y with the given float and return a new Vec2f as shown:
- return Vec2f( this.x * float, this.y * float );

### float opMul( const Vec2f&in )
This will multiply the current Vec2f x and y with the given Vec2f as and return a new float as shown:
- return float( this.x * other.x + this.y * other.y )

### Vec2f& opMulAssign( const Vec2f&in )
This will do opMul and opAssign

### Vec2f& opMulAssign( const float )
This will do opMul and opAssign


## Vec2f opAdd(const Vec2f&in)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f& opAddAssign(const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f opSub(const Vec2f&in)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f& opSubAssign(const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f opDiv(float)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f& opDivAssign(const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& opDivAssign(const float)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f opNeg()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## string opAdd(const string&in)

<br>
<small>Returns: $string </small>

<br>
<br>

## string opAdd_r(const string&in)

<br>
<small>Returns: $string </small>

<br>
<br>

## string toString()

<br>
<small>Returns: $string </small>

<br>
<br>

## bool opEquals(const Vec2f&in)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool opCmp(const Vec2f&in)

<br>
<small>Returns: $bool </small>

<br>
<br>

## float Angle()

<br>
<small>Returns: $float </small>

<br>
<br>

## float AngleDegrees()

<br>
<small>Returns: $float </small>

<br>
<br>

## float AngleRadians()

<br>
<small>Returns: $float </small>

<br>
<br>

## float Length()

<br>
<small>Returns: $float </small>

<br>
<br>

## float LengthSquared()

<br>
<small>Returns: $float </small>

<br>
<br>

## float Normalize()

<br>
<small>Returns: $float </small>

<br>
<br>

## void SetZero()

<br>
<small>Returns: $void </small>

<br>
<br>

## void Set(float, float)

<br>
<small>Returns: $void </small>

<br>
<br>

## float AngleWith(const Vec2f&in)

<br>
<small>Returns: $float </small>

<br>
<br>

## float AngleWithDegrees(const Vec2f&in)

<br>
<small>Returns: $float </small>

<br>
<br>

## float AngleWithRadians(const Vec2f&in)

<br>
<small>Returns: $float </small>

<br>
<br>

## Vec2f& RotateBy(float)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& RotateBy(float, const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& RotateByDegrees(float)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& RotateByDegrees(float, const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& RotateByRadians(float)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## Vec2f& RotateByRadians(float, const Vec2f&in)

<br>
<small>Returns: $Vec2f& </small>

<br>
<br>

## bool isValid()

<br>
<small>Returns: $bool </small>

<br>
<br>

## float getAngle()

<br>
<small>Returns: $float </small>

<br>
<br>

## float getAngleDegrees()

<br>
<small>Returns: $float </small>

<br>
<br>

## float getAngleRadians()

<br>
<small>Returns: $float </small>

<br>
<br>

## float getLength()

<br>
<small>Returns: $float </small>

<br>
<br>

## float getLengthSquared()

<br>
<small>Returns: $float </small>

<br>
<br>

