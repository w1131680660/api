# ColorQuad
------------------------------------------------------------------------------------------
## 描述

存储颜色值的变量
注意：构造之后只读，对于实例中的 R/G/B/A 进行修改是无意义的

------------------------------------------------------------------------------------------
## 属性

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
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
--同ColorValue的区别是 取值区间是0-255
local color = ColorQuad.New(100,100,100,255)

print("color R:"..tostring(color.R).." G:"..tostring(color.G).." B:"..tostring(color.B).." A:"..tostring(color.A))
--color R:100 G:100 B:100 A:255
```