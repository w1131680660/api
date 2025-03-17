# UIButton

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Icon</font></div>|
|:---|
|按钮资源路径|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Title</font></div>|
|:---|
|按钮文字|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TitleSize</font></div>|
|:---|
|按钮文本字体大小|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DownEffectValue</font></div>|
|:---|
|按钮按下效果变化值|

|<div style="width:700px">[DownEffect](/Api/Enums/DownEffect.md) &emsp;<font color="dd00dd">DownEffect</font></div>|
|:---|
|按钮按下效果，有缩放，颜色变化|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Alpha</font></div>|
|:---|
|为1时不透明|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">OutlineEnable</font></div>|
|:---|
|按钮边框是否显示|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">OutlineColor</font></div>|
|:---|
|按钮边框颜色|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">OutlineSize</font></div>|
|:---|
|按钮边框宽度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ShadowEnable</font></div>|
|:---|
|开启按钮阴影|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ShadowColor</font></div>|
|:---|
|按钮阴影颜色|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ShadowOffset</font></div>|
|:---|
|按钮阴影偏移|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsAutoSize</font></div>|
|:---|
|自动大小。为true时，将节点大小调整为图片原本大小|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">IconColor</font></div>|
|:---|
|按钮图片颜色|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ResourceSize</font></div>|
|:---|
|资源尺寸|

|<div style="width:700px">[ScaleType](/Api/Enums/ScaleType.md) &emsp;<font color="dd00dd">ScaleType</font></div>|
|:---|
|按钮图片显示类型：伸缩；裁剪|

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">Scale9Grid</font></div>|
|:---|
|按钮图片九宫格展示|

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">EditAutoSize</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TitleColor</font></div>|
|:---|
|字体颜色|

|<div style="width:700px">[TextVAlignment](/Api/Enums/TextVAlignment.md) &emsp;<font color="dd00dd">TextVAlignment</font></div>|
|:---|
|上下对齐，有向上、中间和向下对齐|

|<div style="width:700px">[TextHAlignment](/Api/Enums/TextHAlignment.md) &emsp;<font color="dd00dd">TextHAlignment</font></div>|
|:---|
|左右对齐，有向左、中间和向右对齐|

|<div style="width:700px">[SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) &emsp;<font color="dd00dd">Press</font></div>|
|:---|
|button按下时候的音效|

|<div style="width:700px">[SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) &emsp;<font color="dd00dd">Release</font></div>|
|:---|
|button抬起时候的音效|

## 代码示例

```lua
--创建ui布局
local root = SandboxNode.new('UIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建按钮
local button= SandboxNode.new('UIButton', game.WorkSpace.uiroot)
button.Icon = 'ui\\mobile\\texture0\\common\\board_activity_box_white.png'
button.Title = "Button"
button.TitleSize = 36
button.DownEffect = Enum.DownEffect.ScaledEffect
button.Size = Vector2.new(100, 50)
button.Position = Vector2.new(200, 100)
button.Alpha= 1
--设置开启描边
button.OutlineEnable= true
--设置开启阴影
button.ShadowEnable= true
```