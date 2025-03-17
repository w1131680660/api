# UITextLabel

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

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FontSize</font></div>|
|:---|
|字体大小|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Title</font></div>|
|:---|
|文本内容|

|<div style="width:700px">[AutoSizeType](/Api/Enums/AutoSizeType.md) &emsp;<font color="dd00dd">IsAutoSize</font></div>|
|:---|
|自动调整节点大小为字体大小|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">OutlineEnable</font></div>|
|:---|
|是否显示边框|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">OutlineColor</font></div>|
|:---|
|边框颜色|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">OutlineSize</font></div>|
|:---|
|边框宽度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ShadowEnable</font></div>|
|:---|
|是否显示阴影|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ShadowColor</font></div>|
|:---|
|阴影颜色|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ShadowOffset</font></div>|
|:---|
|阴影偏移值|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">RichText</font></div>|
|:---|
|超文本|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LineSpacing</font></div>|
|:---|
|行间距|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoTranslator</font></div>|
|:---|
|是否开启自动翻译|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LetterSpacing</font></div>|
|:---|
|字间距|

## 成员函数

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetTextSize</font>](/Api/Classes/Scene/UITextLabel_F/GetTextSize.md) ()</div>|
|:---|
|获取文本宽高尺寸|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local root = SandboxNode.new('UIRoot', workspace)
local label = SandboxNode.new('UITextLabel', root)
label.Title = "商店"
--设置背景框
label.LineColor = ColorQuad.new(0, 0, 0, 0)
--设置背景颜色
label.FillColor = ColorQuad.new(0, 0, 0, 0)
--设置字体颜色
label.TitleColor = ColorQuad.new(255, 0, 0, 255)
--设置位置
label.Position = Vector2.new(75,50)
--设置字体大小
label.FontSize = 18
--设置上下居中对齐
label.TextVAlignment = Enum.TextVAlignment.Center
--设置左右向左对齐
label.TextHAlignment = Enum.TextHAlignment.Left

--设置自动调整大小
label.IsAutoSize= true

--设置开启描边
label.OutlineEnable= true
--设置开启阴影
label.ShadowEnable= true
--获取字体大小
local size = label:GetTextSize()
```