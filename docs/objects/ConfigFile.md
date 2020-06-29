# ConfigFile@ class

---

## <constructor>()

<br>
<small>Returns: $<constructor>() </small>

<br>
<br>

## <constructor>(const string&in)

<br>
<small>Returns: $<constructor>(const </small>

<br>
<br>

## ConfigFile& opAssign(const ConfigFile&in)

<br>
<small>Returns: $ConfigFile& </small>

<br>
<br>

## bool loadFile(string file)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool saveFile(string file)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void remove(const string&in key)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool exists(const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_f32(string key, const float&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_f32(string key, const float[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## float read_f32(const string&in key)

<br>
<small>Returns: $float </small>

<br>
<br>

## float read_f32(const string&in key, const float&in value)

<br>
<small>Returns: $float </small>

<br>
<br>

## bool readIntoArray_f32(float[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_u16(string key, const uint16&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_u16(string key, const uint16[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint16 read_u16(const string&in key)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## uint16 read_u16(const string&in key, const uint16&in value)

<br>
<small>Returns: $uint16 </small>

<br>
<br>

## bool readIntoArray_u16(uint16[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_s16(string key, const int16&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_s16(string key, const int16[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## int16 read_s16(const string&in key)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## int16 read_s16(const string&in key, const int16&in value)

<br>
<small>Returns: $int16 </small>

<br>
<br>

## bool readIntoArray_s16(int16[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_u32(string key, const uint&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_u32(string key, const uint[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint read_u32(const string&in key)

<br>
<small>Returns: $uint </small>

<br>
<br>

## uint read_u32(const string&in key, const uint&in value)

<br>
<small>Returns: $uint </small>

<br>
<br>

## bool readIntoArray_u32(uint[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_s32(string key, const int&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_s32(string key, const int[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## int read_s32(const string&in key)

<br>
<small>Returns: $int </small>

<br>
<br>

## int read_s32(const string&in key, const int&in value)

<br>
<small>Returns: $int </small>

<br>
<br>

## bool readIntoArray_s32(int[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_u8(string key, const uint8&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_u8(string key, const uint8[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## uint8 read_u8(const string&in key)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## uint8 read_u8(const string&in key, const uint8&in value)

<br>
<small>Returns: $uint8 </small>

<br>
<br>

## bool readIntoArray_u8(uint8[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_s8(string key, const int8&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_s8(string key, const int8[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## int8 read_s8(const string&in key)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## int8 read_s8(const string&in key, const int8&in value)

<br>
<small>Returns: $int8 </small>

<br>
<br>

## bool readIntoArray_s8(int8[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_bool(string key, const bool&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_bool(string key, const bool[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## bool read_bool(const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool read_bool(const string&in key, const bool&in value)

<br>
<small>Returns: $bool </small>

<br>
<br>

## bool readIntoArray_bool(bool[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void add_string(string key, const string&in value)

<br>
<small>Returns: $void </small>

<br>
<br>

## void addArray_string(string key, const string[]&in arr)

<br>
<small>Returns: $void </small>

<br>
<br>

## string read_string(const string&in key)

<br>
<small>Returns: $string </small>

<br>
<br>

## string read_string(const string&in key, const string&in value)

<br>
<small>Returns: $string </small>

<br>
<br>

## bool readIntoArray_string(string[]&inout arr, const string&in key)

<br>
<small>Returns: $bool </small>

<br>
<br>

## void ExtractToBitStream(CBitStream&inout bt)

<br>
<small>Returns: $void </small>

<br>
<br>

