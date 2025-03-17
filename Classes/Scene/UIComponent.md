# UIComponent

## 描述

按需加载fairygui::GGraph

## 属性

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Size</font></div>|
|:---|
|UI节点像素和尺寸大小|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Scale</font></div>|
|:---|
|UI节点缩放倍数|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Rotation</font></div>|
|:---|
|UI节点旋转度数|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|UI节点坐标|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Pivot</font></div>|
|:---|
|UI节点锚点（0~1），（0.5,0.5）为中点|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsKeepPosWhenPivotChange</font></div>|
|:---|
|更新锚点时是否保持位置不变|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsNotifyEventStop</font></div>|
|:---|
|是否将触摸事件传递给父节点（为true时不传递）|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LineColor</font></div>|
|:---|
|UI节点边线颜色设置|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">FillColor</font></div>|
|:---|
|UI节点填充颜色设置|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LineSize</font></div>|
|:---|
|UI节点边线像素和尺寸大小|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ClickPass</font></div>|
|:---|
|是否将点击事件穿透给场景|

|<div style="width:700px">[EnumLayoutHRelation](/Api/Enums/EnumLayoutHRelation.md) &emsp;<font color="dd00dd">LayoutHRelation</font></div>|
|:---|
|水平关联方式，包括左关联、中线关联和右关联。设置后，当父节点（若父节点为UIRoot则为屏幕）变化时，UI与关联位置的相对距离将保持不变|

|<div style="width:700px">[EnumLayoutVRelation](/Api/Enums/EnumLayoutVRelation.md) &emsp;<font color="dd00dd">LayoutVRelation</font></div>|
|:---|
|垂直关联方式，包括上关联、中线关联和下关联。设置后，当父节点（若父节点为UIRoot则为屏幕）变化时，UI与关联位置的相对距离将保持不变|

|<div style="width:700px">[EnumLayoutSizeRelation](/Api/Enums/EnumLayoutSizeRelation.md) &emsp;<font color="dd00dd">LayoutSizeRelation</font></div>|
|:---|
|宽高关联，包括无关联，宽关联，高关联和全关联，当父节点宽高改变时，UI宽高随之变化|

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetFullViewSize</font></div>|
|:---|
|设置全视图大小|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Active</font></div>|
|:---|
|是否激活(响应点击时间)|

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetLeftAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetRightAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetHorizontalAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetTopAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetBottomAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetVerticalAlign</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetEqualWidth</font></div>|
|:---|
||

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">SetEqualHeight</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Grayed</font></div>|
|:---|
|置灰|

## 成员函数

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetGlobalPos</font>](/Api/Classes/Scene/UIComponent_F/GetGlobalPos.md) ()</div>|
|:---|
|获取UI的全局位置|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RollOver</font>](/Api/Classes/Scene/UIComponent_F/RollOver.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isOver, [Vector2](/Api/DataType/Vector2.md) vector2)</div>|
|:---|
|鼠标进入UI范围|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RollOut</font>](/Api/Classes/Scene/UIComponent_F/RollOut.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isOut, [Vector2](/Api/DataType/Vector2.md) vector2)</div>|
|:---|
|鼠标超出UI范围|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TouchBegin</font>](/Api/Classes/Scene/UIComponent_F/TouchBegin.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isTouchBegin, [Vector2](/Api/DataType/Vector2.md) vector2, [int](/Api/DataType/Number.md) int)</div>|
|:---|
|触摸事件开始|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TouchEnd</font>](/Api/Classes/Scene/UIComponent_F/TouchEnd.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isTouchEnd, [Vector2](/Api/DataType/Vector2.md) vector2, [int](/Api/DataType/Number.md) int)</div>|
|:---|
|触摸事件结束|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TouchMove</font>](/Api/Classes/Scene/UIComponent_F/TouchMove.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isTouchMove, [Vector2](/Api/DataType/Vector2.md) vector2, [int](/Api/DataType/Number.md) int)</div>|
|:---|
|触摸移动|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Click</font>](/Api/Classes/Scene/UIComponent_F/Click.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isClick, [Vector2](/Api/DataType/Vector2.md) vector2, [int](/Api/DataType/Number.md) int)</div>|
|:---|
|点击事件|

## 代码示例

```lua
--创建ui布局
local root = SandboxNode.new('UIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建图片
local image1 = SandboxNode.new('UIImage', game.WorkSpace.uiroot)
image1.Name = 'image'
image1.Visible = true
image1.Icon = 'ui\\mobile\\texture0\\common\\board_activity_box_white.png'
image1.Size = Vector2.new(500, 200)
image1.Pivot= Vector2.new(0, 0)
image1.LayoutHRelation = Enum.LayoutHRelation.Left
image1.LayoutVRelation= Enum.LayoutVRelation.Top
image1.LayoutSizeRelation= Enum.LayoutSizeRelation.Both

image1.RollOver:connect(function(node,issuccess,mousepos)
	print('you RollOver me')
	print('RollOver pos:'..mousepos.x..' '..mousepos.y)
end)
image1.RollOut:connect(function(node,issuccess,mousepos)
	print('you RollOut me')
	print('RollOut pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchBegin:connect(function(node,issuccess,mousepos)
	print('you TouchBegin me')
	print('TouchBegin pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchMove:connect(function(node,issuccess,mousepos)
	print('you TouchMove me')
	print('TouchMove pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchEnd:connect(function(node,issuccess,mousepos)
	print('you TouchEnd me')
	print('TouchEnd pos:'..mousepos.x..' '..mousepos.y)
end)
image1.Click:connect(function(node,issuccess,mousepos)
	print('you Clickme')
	print('Clickme pos:'..mousepos.x..' '..mousepos.y)
end)
```