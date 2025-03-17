# ColorValue
------------------------------------------------------------------------------------------
## 描述

存储颜色值的变量
注意：构造之后只读，对于实例中的 R/G/B/A 进行修改是无意义的

------------------------------------------------------------------------------------------
## 属性

|<div style="width:700px">[ColorValue](/Api/DataType/ColorValue.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
|:---|
|构造|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">R</font>]()</div>|
|:---|
|红|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">G</font>]()</div>|
|:---|
|绿|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">B</font>]()</div>|
|:---|
|蓝|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">A</font>]()</div>|
|:---|
|透明度|

------------------------------------------------------------------------------------------
## 示例代码

```lua
--同ColorQuad的区别是 取值区间是0-1.0f
local color = ColorValue.New(0,0,0,0.0f)

print("color R:"..tostring(color.R).." G:"..tostring(color.G).." B:"..tostring(color.B).." A:"..tostring(color.A))
--color R:0 G:0 B:0 A:0.0f
```