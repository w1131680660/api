# UITextInput

## 属性

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TitleColor</font></div>|
|:---|
|字体颜色|

|<div style="width:700px">[TextVAlignment](/Api/Enums/TextVAlignment.md) &emsp;<font color="dd00dd">TextVAlignment</font></div>|
|:---|
|上下对齐，有向上、中间和向下对齐|

|<div style="width:700px">[TextHAlignment](/Api/Enums/TextHAlignment.md) &emsp;<font color="dd00dd">TextHAlignment</font></div>|
|:---|
|左右对齐，有向左、中间和向右对齐|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">MaxLength</font></div>|
|:---|
|限制输入文本长度|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FontSize</font></div>|
|:---|
|字体大小|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Title</font></div>|
|:---|
|输入的文本内容|

|<div style="width:700px">[InputMode](/Api/Enums/InputMode.md) &emsp;<font color="dd00dd">Input</font></div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Return</font>](/Api/Classes/Scene/UITextInput_F/Return.md) ([bool](/Api/DataType/Bool.md) onReturn)</div>|
|:---|
|输入完成时触发|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local root= SandboxNode.new('UIRoot', workspace)
local petNameText = SandboxNode.new('UITextInput', root)
--设置节点名字
petNameText.Name = "PetNameText"
--设置节点大小
petNameText.Size = Vector2.new(120, 50)
--设置节点位置
petNameText.Position = Vector2.new(400, 250)
--设置是否可见
petNameText.Visible = true
--设置输入框背景颜色
petNameText.FillColor = ColorQuad.new(97, 151, 230, 255)
--设置文本上下对齐
petNameText.TextVAlignment = Enum.TextVAlignment.Center
--设置文本左右对齐
petNameText.TextHAlignment = Enum.TextHAlignment.Center
--设置输入内容
petNameText.Title = "宠物狼"
--设置输入文本最长长度
petNameText.MaxLength = 20
--设置输入文本字体大小
petNameText.FontSize = 25
```