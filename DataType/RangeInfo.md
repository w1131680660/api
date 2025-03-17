# RangeInfo
------------------------------------------------------------------------------------------
## 描述

范围数据类型，包含四个属性:
- Min
- Max

注意：构造之后只读

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
|:---|
|构造|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Min</font>]()</div>|
|:---|
|范围最小值|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Max</font>]()</div>|
|:---|
|范围最大值|


------------------------------------------------------------------------------------------
## 代码示例

```lua
local range = range.New(0,10)
print("Min:"..tostring(rect.Min).." Max:"..tostring(rect.Max))
--Min:0 Max:10
```