# CBitStream@ class

---

## <constructor>()

<br>
<small>Returns: $<constructor>() </small>

<br>
<br>

## void write_s8(int8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int8 read_s8()

<br>
<small>Returns: $int8 </small>

<br>
<br>

## bool saferead_s8(int8&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_u8(uint8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint8 read_u8()

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## bool saferead_u8(uint8&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_s16(int16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int16 read_s16()

<br>
<small>Returns: $int16 </small>

<br>
<br>

## bool saferead_s16(int16&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_u16(uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 read_u16()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## bool saferead_u16(uint16&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_netid(uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 read_netid()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## bool saferead_netid(uint16&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_s32(int v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int read_s32()

<br>
<small>Returns: $int </small>

<br>
<br>

## bool saferead_s32(int&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_u32(uint v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint read_u32()

<br>
<small>Returns: $uint </small>

<br>
<br>

## bool saferead_u32(uint&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_f32(float v)

<br>
<small>Returns: $void </small>

<br>
<br>

## float read_f32()

<br>
<small>Returns: $float </small>

<br>
<br>

## bool saferead_f32(float&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_bool(bool v)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool read_bool()

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool saferead_bool(bool&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_string(string str)

<br>
<small>Returns: $void </small>

<br>
<br>

## string read_string()

<br>
<small>Returns: $string </small>

<br>
<br>

## bool saferead_string(string&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_Vec2f(Vec2f v)

<br>
<small>Returns: $void </small>

<br>
<br>

## Vec2f read_Vec2f()

<br>
<small>Returns: $Vec2f </small>

<br>
<br>

## bool saferead_Vec2f(Vec2f&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void write_TileType(uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 read_TileType()

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## bool saferead_TileType(uint16&out)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void overwrite_at_bit_s8(uint bit, int8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int8 read_at_bit_s8(uint byte)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## void overwrite_at_bit_u8(uint bit, uint8 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint8 read_at_bit_u8(uint byte)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## void overwrite_at_bit_s16(uint bit, int16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int16 read_at_bit_s16(uint byte)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## void overwrite_at_bit_u16(uint bit, uint16 v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 read_at_bit_u16(uint byte)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## void overwrite_at_bit_s32(uint bit, int v)

<br>
<small>Returns: $void </small>

<br>
<br>

## int read_at_bit_s32(uint byte)

<br>
<small>Returns: $int </small>

<br>
<br>

## void overwrite_at_bit_u32(uint bit, uint v)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint read_at_bit_u32(uint byte)

<br>
<small>Returns: $uint </small>

<br>
<br>

## void overwrite_at_bit_f32(uint bit, float v)

<br>
<small>Returns: $void </small>

<br>
<br>

## float read_at_bit_f32(uint byte)

<br>
<small>Returns: $float </small>

<br>
<br>

## void ResetBitIndex()

<br>
<small>Returns: $void </small>

<br>
<br>

## void Reset()

<br>
<small>Returns: $void </small>

<br>
<br>

## void SetBitIndex(uint Index)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint getBitIndex()

<br>
<small>Returns: $uint </small>

<br>
<br>

## void ResetBuffer()

<br>
<small>Returns: $void </small>

<br>
<br>

## void Clear()

<br>
<small>Returns: $void </small>

<br>
<br>

## uint getBitsUsed()

<br>
<small>Returns: $uint </small>

<br>
<br>

## uint getBytesUsed()

<br>
<small>Returns: $uint </small>

<br>
<br>

## uint Length()

<br>
<small>Returns: $uint </small>

<br>
<br>

## bool isBufferEnd()

<br>
<small>Returns: $bool </small>

<br>
<br>

## void writeBitStream(CBitStream@ bitstream)

<br>
<small>Returns: $void </small>

<br>
<br>

## void write_CBitStream(CBitStream@ bitstream)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool saferead_CBitStream(CBitStream@ bitstream)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void writeBitStream(CBitStream@ bitstream, int index, int bits)

<br>
<small>Returns: $void </small>

<br>
<br>

## CBitStream& opAssign(const CBitStream&in)

<br>
<small>Returns: $CBitStream& </small>

<br>
<br>

## void Compress(int level)

<br>
<small>Returns: $void </small>

<br>
<br>

## void Decompress()

<br>
<small>Returns: $void </small>

<br>
<br>

