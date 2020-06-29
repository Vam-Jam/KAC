# CGridMenu@ class

---

## bool deleteAfterClick

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool modal

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool kill

<br>
<small>Returns: $bool </small>

<br>
<br>

## CBlob@ getOwner()

<br>
<small>Returns: $CBlob@ </small>

<br>
<br>

## string getName()

<br>
<small>Returns: $string </small>

<br>
<br>

## int getButtonsCount()

<br>
<small>Returns: $int </small>

<br>
<br>

## CGridButton@ getButtonOfIndex(int index)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(CGridButton@ button)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconTexture, int frame, const string&in caption, uint8 cmdID)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconTexture, int frame, const string&in caption, uint8 cmdID, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconTexture, int frame, const string&in caption, uint8 cmdID, Vec2f slotsDim)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconTexture, int frame, const string&in caption, uint8 cmdID, Vec2f slotsDim, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconTexture, int frame, Vec2f frameDimension, const string&in caption, uint8 cmdID, Vec2f slotsDim, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconName, const string&in caption, uint8 cmdID)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconName, const string&in caption, uint8 cmdID, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconName, const string&in caption, uint8 cmdID, Vec2f slotsDim)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconName, const string&in caption, uint8 cmdID, Vec2f slotsDim, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddButton(const string&in iconName, const string&in caption, Vec2f slotsDim)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddTextButton(const string&in caption, Vec2f slotsDim)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddTextButton(const string&in caption, uint8 cmdID, Vec2f slotsDim, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddItemButton(CBlob@ blob, uint8 cmdID)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddItemButton(CBlob@ blob, uint8 cmdID, CBitStream&in parameters)

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## CGridButton@ AddEmptyButton()

<br>
<small>Returns: $CGridButton@ </small>

<br>
<br>

## void FillUpRow()

<br>
<small>Returns: $void </small>

<br>
<br>

## bool RemoveButton(CGridButton@ button)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool DeleteButton(CGridButton@ button)

<br>
<small>Returns: $bool </small>

<br>
<br>

## Vec2f getUpperLeftPosition()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## Vec2f getLowerRightPosition()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## void SetDefaultCommand(uint8 cmd, CBitStream&in parameters)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetCaptionEnabled(bool enabled)

<br>
<small>Returns: $void </small>

<br>
<br>

## void AddKeyCommand(EKEY_CODE key, uint8 cmdID, CBitStream&in parameters)

<br>
<small>Returns: $void </small>

<br>
<br>

