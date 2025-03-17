# Rect
------------------------------------------------------------------------------------------
## 描述

矩形数据类型，包含四个属性:
- Left
- Right
- Top
- Bottom

注意：构造之后只读

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:700px">[Rect](/Api/DataType/Rect.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
|:---|
|构造|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Left</font>]()</div>|
|:---|
|矩形左边的X坐标|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Right</font>]()</div>|
|:---|
|矩形右边的X坐标|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Top</font>]()</div>|
|:---|
|矩形顶部的Y坐标|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Bottom</font>]()</div>|
|:---|
|矩形底部的Y坐标|

------------------------------------------------------------------------------------------
## 代码示例

```lua
local rect = Rect.New(0,1,2,3)
print("Left:"..tostring(rect.Left).." Right:"..tostring(rect.Right).." Top:"..tostring(rect.Top).." Bottom:"..tostring(rect.Bottom))
--Left:0 Right:2 Top:1 Bottom:3
```