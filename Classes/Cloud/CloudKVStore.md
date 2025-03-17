# CloudKVStore

## 成员函数

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetTopSync</font>](/Api/Classes/Cloud/CloudKVStore_F/GetTopSync.md) ([int](/Api/DataType/Number.md) count)</div>|
|:---|
|获取排行榜Top数据|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetBottomSync</font>](/Api/Classes/Cloud/CloudKVStore_F/GetBottomSync.md) ([int](/Api/DataType/Number.md) count)</div>|
|:---|
|获取排行榜Bottom数据|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetRangeSync</font>](/Api/Classes/Cloud/CloudKVStore_F/GetRangeSync.md) ([int](/Api/DataType/Number.md) , [bool](/Api/DataType/Bool.md) , [int](/Api/DataType/Number.md) , [int](/Api/DataType/Number.md) )</div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetOrderDataIndex</font>](/Api/Classes/Cloud/CloudKVStore_F/GetOrderDataIndex.md) ([bool](/Api/DataType/Bool.md) bAscend, [int](/Api/DataType/Number.md) nIndex)</div>|
|:---|
|获取排行榜名次|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">CleanOrderDataList</font> ()</div>|
|:---|
|replace|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clean</font> ()</div>|
|:---|
|清理排行榜数据|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">SetValue</font>](/Api/Classes/Cloud/CloudKVStore_F/SetValue.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name, [int](/Api/DataType/Number.md) value)</div>|
|:---|
|设置同步kv值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetValue</font>](/Api/Classes/Cloud/CloudKVStore_F/GetValue.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name)</div>|
|:---|
|获取同步kv值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">SetValueAsync</font>](/Api/Classes/Cloud/CloudKVStore_F/SetValueAsync.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name, [int](/Api/DataType/Number.md) value, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|设置异步kv值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetValueAsync</font>](/Api/Classes/Cloud/CloudKVStore_F/GetValueAsync.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) value, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取异步kv值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">RemoveKey</font>](/Api/Classes/Cloud/CloudKVStore_F/RemoveKey.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|同步移除kv值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">RemoveKeyAsync</font>](/Api/Classes/Cloud/CloudKVStore_F/RemoveKeyAsync.md) ([string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) arg2)</div>|
|:---|
|异步移除kv值|

## 代码示例

```lua
local CloudService = game:GetService("CloudService")

--获取排行榜（没有则创建）
 local Level = CloudService:GetOrderDataCloud("LevelAA")
--清空排行榜
Level:CleanOrderDataList()

 local LeveBB= CloudService:GetOrderDataCloud("LevelBB")

--同步设值
LeveBB:SetValue("1000068432","无意义",40)
LeveBB:SetValue("1000038432","无意义",70)
print("Hello LeveBB!")

--异步设值
LeveBB:SetValueAsync("1000018432","无意义",50, function (code)
	--code 为0成功，非0失败
	print("code is ", code)
end)

LeveBB:SetValueAsync("1000028432","无意义",60, function (code)
	--code 为0成功，非0失败
	print("code is ", code)
end)

LeveBB:SetValueAsync("1000048432","无意义",70, function (code)
	--code 为0成功，非0失败
	print("code is ", code)
end)


--同步获值
local getVal = LeveBB:GetValue("1000068432","无意义")
print("getVal is!", getVal)

local newGetVal = LeveBB:GetValueAsync("1000068432","无意义", function (code, val)
	--code 为0成功，非0失败
	print("code is, getVal is ", code, val)
end)
print("Hello LeveBB!")

--获取降序第二名
 local tableA = LeveBB:GetOrderDataIndex(false, 2)
for k, v in pairs(tableA) do
	print("TABLE A    key is value is", v.key,  v.value)
end
print("Hello LeveBB!")

--获取降序第二名到四名
 local  tableB = LeveBB:GetOrderDataValueArea(false, 2, 4)
for k, v in pairs(tableB) do
	print("TABLE B  key is value is", v.key,  v.value)
end

```