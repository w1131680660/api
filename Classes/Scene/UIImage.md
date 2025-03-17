# UIImage

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Icon</font></div>|
|:---|
|图片资源路径|

|<div style="width:700px">[EnumFillMethod](/Api/Enums/EnumFillMethod.md) &emsp;<font color="dd00dd">FillMethod</font></div>|
|:---|
|填充模式|

|<div style="width:700px">[EnumFillOrigin](/Api/Enums/EnumFillOrigin.md) &emsp;<font color="dd00dd">FillOrigin</font></div>|
|:---|
|填充原点（仅在Horizontal与Vertical填充模式下适用）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">FillClockwise</font></div>|
|:---|
|顺时针填充（仅在Radial360模式下适用），为true时以上方中点为起点，根据FillAmount比例顺时针渲染，否则为逆时针|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FillAmount</font></div>|
|:---|
|填充比例（0~1），填充显示的部分占原来大小的比例|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsAutoSize</font></div>|
|:---|
|自动大小。为true时，将节点大小调整为图片原本大小|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Alpha</font></div>|
|:---|
|为1时不透明|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ResourceSize</font></div>|
|:---|
|资源大小|

|<div style="width:700px">[ScaleType](/Api/Enums/ScaleType.md) &emsp;<font color="dd00dd">ScaleType</font></div>|
|:---|
|比例类型|

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">Scale9Grid</font></div>|
|:---|
|图片比例九宫格|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoTranslator</font></div>|
|:---|
|是否开启自动翻译|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">BlurFilter</font></div>|
|:---|
|是否开启高斯模糊|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">BlurSigma</font></div>|
|:---|
|高斯模糊sigma(取值范围1-5)|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">UIMaskMode</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">EditAutoSize</font></div>|
|:---|
||

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">TextureRect</font></div>|
|:---|
||

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local name = SandboxNode.new('UIList', workspace)

--设置排列方式
name.ScrollType = Enum.ListLayoutType.FLOW_HORIZONTAL
name.OverflowType = Enum.OverflowType.HORIZONTAL
--设置行数列数
name.LineCount = 2
name.ColumnCount = 2

--设置行距列距
name.LineGap= 50
name.ColumnGap= 50

--设置自动调整项目大小
name.AutoResizeItem= true

--设置上下居中对齐
name.HorizontalAlign= Enum.TextVAlignment.Center
--设置左右向左对齐
name.VerticalAlign= Enum.TextHAlignment.Left

--设置虚拟循环列表
name.SetVirtualAndLoop
```