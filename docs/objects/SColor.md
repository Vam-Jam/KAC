# SColor class
SColor class is used to contain color.
<br>
The most important thing to know about this class is that the color is set following an ARGB pattern : 0xAARRGGBB

+ The values range from 0 to 255.
+ `SColor(alpha, red, green, blue);`

---

## \<constructor>()
All values in SColor are by default 0 when nothing is specified.

<br>

## void set(uint)
## \<constructor>(uint)
Sets a hex value.
SColor accepts hex values. For example, the color `(255, 211, 249, 193)`
can be expressed as `(0xFFD3F9C1)`
This can be assigned to an SColor variable via its constructor like this `SColor(0xFFD3F9C1)`
This can be assigned to an SColor variable after initialization like this `color.set(0xFFD3F9C1);`

Remember to include the two digits that represent the alpha value.

This is used quite a bit in vanilla KAG, there is no advantage/disavatnage of doing this way.

<br>

## void set(uint, uint, uint, uint)
## \<constructor>(uint, uint, uint, uint)

Sets the alpha, red, blue, and green of the SColor variable.

**Parameters**
1. Alpha - How visible the color is. (results can vary depending on what is using this)
2. Red - How much red the color has.
3. Blue - How much blue the color has.
4. Green - How much green the color has.
### Examples
`color.set(255, 255, 0 ,0)` Used to assign a red color to an existing SColor variable.
`SColor(255, 255, 0, 0);` for a red color on creation of a SColor variable.

<br>

## \<constructor>(SColor)
SColor can be initialized with another SColor.

**Parameters**
1. Another SColor variable.

<br>



## uint getAlpha() const
Returns the alpha value.

255 is fully visible.
127 is half visible.
0 is not visible.
## void setAlpha(uint)
Sets the alpha value.

<br>


## uint getRed() const
Returns the red value.

<br>

## void setRed(uint)
Sets the amount of red.

<br>

## uint getGreen() const
Returns the green value

<br>

## void setGreen(uint)
Sets the amount of green.

<br>

## uint getBlue() const
Returns the blue value.

<br>

## void setBlue(uint)
Sets the amount of blue.

<br>

## uint getAverage() const

<br>

## float getLuminance() const

<br>

## SColor getInterpolated(const SColor&in, float) const

<br>

## SColor getInterpolated_quadratic(const SColor&in, const SColor&in, float) const

<br>

## SColor& opAssign(const SColor&in)

<br>

## SColor opAdd(const SColor&in)

<br>

## bool opEquals(const SColor&in)

<br>

## bool opCmp(const SColor&in)

<br>


## Usage Example
```as
void onRender( CRules@ this )
{
	SColor background_color = SColor(127, 255, 0, 0);//Red
	GUI::DrawRectangle(Vec2f(0, 0), Vec2f(500, 500), background_color);

  background_color.setBlue(255);//Makes the blue value 255, turning the color purple.
  GUI::DrawRectangle(Vec2f(500, 500), Vec2f(1000, 1000), background_color);
}
```
From the top left this draws a rectangle stretching 500 down and 500 right as a red color with half opacity. After that is done, it sets the blue value to 255 turning background_color purple. After that happens, another rectangle is drawn to demonstrate that the color is purple.
