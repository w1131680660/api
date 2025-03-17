# ClickDetector

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MouseClick</font>](/Api/Classes/Input/ClickDetector_F/MouseClick.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标左键点击节点时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RightMouseClick</font>](/Api/Classes/Input/ClickDetector_F/RightMouseClick.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标右键点击时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MouseHoverEnter</font>](/Api/Classes/Input/ClickDetector_F/MouseHoverEnter.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标停在节点上时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MouseHoverLeave</font>](/Api/Classes/Input/ClickDetector_F/MouseHoverLeave.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标在节点上离开时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MouseDown</font>](/Api/Classes/Input/ClickDetector_F/MouseDown.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标按下时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MouseUp</font>](/Api/Classes/Input/ClickDetector_F/MouseUp.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标弹起时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RightMouseDown</font>](/Api/Classes/Input/ClickDetector_F/RightMouseDown.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标右键按下时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RightMouseUp</font>](/Api/Classes/Input/ClickDetector_F/RightMouseUp.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|鼠标右键弹起时触发|

## 代码示例

```lua
--创建模型
local model = SandboxNode.new('Model', game.WorkSpace)
model.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100041")
model.Position = Vector3.new(500, 700, 150)
--绑定点击点
local clickDetector = sandboxNode.new('ClickDetector', model)
--监听MouseClick事件
clickDetector.MouseClick:connect(function()
	print("You clicked me!")
end)
```