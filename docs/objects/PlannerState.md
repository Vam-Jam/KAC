# PlannerState@ class

---

## Vec2f pos

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## string name

<br>
<small>Returns: $string </small>

<br>
<br>

## CBlob@ blob

<br>
<small>Returns: $CBlob@ </small>

<br>
<br>

## CBrain@ brain

<br>
<small>Returns: $CBrain@ </small>

<br>
<br>

## uint8 team

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## CHighMapNode@ highlevelnode

<br>
<small>Returns: $CHighMapNode@ </small>

<br>
<br>

## bool solution

<br>
<small>Returns: $bool </small>

<br>
<br>

## void Print()

<br>
<small>Returns: $void </small>

<br>
<br>

## bool hasSameProperties(PlannerState@ state)

<br>
<small>Returns: $bool </small>

<br>
<br>

## PlannerState& opAssign(const PlannerState&in)

<br>
<small>Returns: $PlannerState& </small>

<br>
<br>

## uint getHashCode() const

<br>
<small>Returns: $uint </small>

<br>
<br>

## void set(const string&in, ?&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool get(const string&in, ?&out) const

<br>
<small>Returns: $bool </small>

<br>
<br>

## void set(const string&in, int64&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool get(const string&in, int64&out) const

<br>
<small>Returns: $bool </small>

<br>
<br>

## void set(const string&in, double&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool get(const string&in, double&out) const

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool getAt(const string&in, int index, ?&out) const

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool getLast(const string&in, ?&out) const

<br>
<small>Returns: $bool </small>

<br>
<br>

## void setAt(const string&in, int index, ?&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## void push(const string&in, ?&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## void removeAt(const string&in, int index)

<br>
<small>Returns: $void </small>

<br>
<br>

## void removeElement(const string&in, ?&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## void clear(const string&in)

<br>
<small>Returns: $void </small>

<br>
<br>

## void debug()

<br>
<small>Returns: $void </small>

<br>
<br>

## bool exists(const string&in)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void set_s8(const string&in, int8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int8 get_s8(const string&in)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## void set_u8(const string&in, uint8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint8 get_u8(const string&in)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## void set_s16(const string&in, int16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int16 get_s16(const string&in)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## void set_u16(const string&in, uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 get_u16(const string&in)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void set_netid(const string&in, uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 get_netid(const string&in)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void set_s32(const string&in, int v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int get_s32(const string&in)

<br>
<small>Returns: $int </small>

<br>
<br>

## void set_u32(const string&in, uint v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint get_u32(const string&in)

<br>
<small>Returns: $uint </small>

<br>
<br>

## void set_f32(const string&in, float v)

<br>
<small>Returns: $void </small>

<br>
<br>

## float get_f32(const string&in)

<br>
<small>Returns: $float </small>

<br>
<br>

## void set_bool(const string&in, bool v)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool get_bool(const string&in)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void set_string(const string&in, string v)

<br>
<small>Returns: $void </small>

<br>
<br>

## string get_string(const string&in)

<br>
<small>Returns: $string </small>

<br>
<br>

## void set_Vec2f(const string&in, Vec2f v)

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f get_Vec2f(const string&in)

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## void set_TileType(const string&in, uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 get_TileType(const string&in)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void set_CBitStream(const string&in, CBitStream&inout bs)

<br>
<small>Returns: $void </small>

<br>
<br>

## void get_CBitStream(const string&in, CBitStream&inout bs)

<br>
<small>Returns: $void </small>

<br>
<br>

## void Sync(const string&in name, bool relayToClients)

<br>
<small>Returns: $void </small>

<br>
<br>

## void SyncToPlayer(const string&in name, CPlayer@ player)

<br>
<small>Returns: $void </small>

<br>
<br>

## void Tag(const string&in name)

<br>
<small>Returns: $void </small>

<br>
<br>

## void Untag(const string&in name)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool hasTag(const string&in name)

<br>
<small>Returns: $bool </small>

<br>
<br>

## int8 add_s8(const string&in, int8 value)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## int8 sub_s8(const string&in, int8 value)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## int16 add_s16(const string&in, int16 value)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## int16 sub_s16(const string&in, int16 value)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## int add_s32(const string&in, int value)

<br>
<small>Returns: $int </small>

<br>
<br>

## int sub_s32(const string&in, int value)

<br>
<small>Returns: $int </small>

<br>
<br>

## uint8 add_u8(const string&in, uint8 value)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## uint8 sub_u8(const string&in, uint8 value)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## uint16 add_u16(const string&in, uint16 value)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## uint16 sub_u16(const string&in, uint16 value)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## uint add_u32(const string&in, uint value)

<br>
<small>Returns: $uint </small>

<br>
<br>

## uint sub_u32(const string&in, uint value)

<br>
<small>Returns: $uint </small>

<br>
<br>

## float add_f32(const string&in, float value)

<br>
<small>Returns: $float </small>

<br>
<br>

## float sub_f32(const string&in, float value)

<br>
<small>Returns: $float </small>

<br>
<br>

