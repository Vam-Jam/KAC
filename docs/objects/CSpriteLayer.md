# CSpriteLayer@ class

---

## string name

<br>
<small>Returns: $string </small>

<br>
<br>

## Animation@ animation

<br>
<small>Returns: $Animation@ </small>

<br>
<br>

## Animation@ getAnimation(const string&in)

<br>
<small>Returns: $Animation@ </small>

<br>
<br>

## void SetAnimation(Animation@ anim)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetAnimation(const string&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isAnimation(const string&in)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool isAnimationEnded()

<br>
<small>Returns: $bool </small>

<br>
<br>

## Animation@ addAnimation(const string&in name, uint16 time, bool loop)

<br>
<small>Returns: $Animation@ </small>

<br>
<br>

## bool isFrame(uint16 frame)

<br>
<small>Returns: $bool </small>

<br>
<br>

## uint16 getFrame()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## uint16 getNextFrameIndex()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void SetFrameIndex(uint16 frame)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetFrame(uint16 sheetindex)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isFrameIndex(uint16 frame)

<br>
<small>Returns: $bool </small>

<br>
<br>

## uint16 getFrameIndex()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void ResetTransform()

<br>
<small>Returns: $void </small>

<br>
<br>

## void TranslateBy(Vec2f p)

<br>
<small>Returns: $void </small>

<br>
<br>

## void RotateBy(float degrees, Vec2f around)

<br>
<small>Returns: $void </small>

<br>
<br>

## void RotateByDegrees(float degrees, Vec2f around)

<br>
<small>Returns: $void </small>

<br>
<br>

## void RotateByRadians(float radians, Vec2f around)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ScaleBy(Vec2f p)

<br>
<small>Returns: $void </small>

<br>
<br>

## void ScaleBy(float x, float y)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetOffset(Vec2f o)

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f getOffset()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## void SetFacingLeft(bool left)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isFacingLeft()

<br>
<small>Returns: $bool </small>

<br>
<br>

## void SetIgnoreParentFacing(bool ignore)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool getIgnoreParentFacing()

<br>
<small>Returns: $bool </small>

<br>
<br>

## void SetVisible(bool visible)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isVisible()

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool SetLighting(bool lighting)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void SetRelativeZ(float z)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetInterpolated(bool value)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool isInterpolated() const

<br>
<small>Returns: $bool </small>

<br>
<br>

## float getRelativeZ()

<br>
<small>Returns: $float </small>

<br>
<br>

## void SetHUD(bool onhud)

<br>
<small>Returns: $void </small>

<br>
<br>

## string getFilename()

<br>
<small>Returns: $string </small>

<br>
<br>

## int getFrameWidth()

<br>
<small>Returns: $int </small>

<br>
<br>

## int getFrameHeight()

<br>
<small>Returns: $int </small>

<br>
<br>

## int getTextureWidth()

<br>
<small>Returns: $int </small>

<br>
<br>

## int getTextureHeight()

<br>
<small>Returns: $int </small>

<br>
<br>

## void SetColor(SColor color)

<br>
<small>Returns: $void </small>

<br>
<br>

## SColor getColor()

<br>
<small>Returns: $SColor </small>

<br>
<br>

## bool ReloadSprite(const string&in filename)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool ReloadSprite(const string&in filename, int frameWidth, int frameHeight)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool ReloadSprite(const string&in filename, int frameWidth, int frameHeight, int teamColor, int skinColor)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool SetTexture(const string&in texture)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool SetTexture(const string&in texture, int frameWidth, int frameHeight)

<br>
<small>Returns: $bool </small>

<br>
<br>

## string getTextureName()

<br>
<small>Returns: $string </small>

<br>
<br>

## void MakeParticle(Vec2f vel, float gravity)

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f getWorldTranslation()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## bool isOnScreen()

<br>
<small>Returns: $bool </small>

<br>
<br>

## void setRenderStyle(Style style)

<br>
<small>Returns: $void </small>

<br>
<br>

