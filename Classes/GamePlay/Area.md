# Area

## 属性

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Beg</font></div>|
|:---|
|起始位置世界坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">End</font></div>|
|:---|
|结束位置世界坐标|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EffectWidth</font></div>|
|:---|
|效果宽度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Show</font></div>|
|:---|
|是否显示|

|<div style="width:700px">[SceneEffectFrameShowMode](/Api/Enums/SceneEffectFrameShowMode.md) &emsp;<font color="dd00dd">ShowMode</font></div>|
|:---|
|显示模式的枚举|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">Color</font></div>|
|:---|
|区域颜色|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">EnterNode</font>](/Api/Classes/GamePlay/Area_F/EnterNode.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|节点进入该区域时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">LeaveNode</font>](/Api/Classes/GamePlay/Area_F/LeaveNode.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|节点离开该区域时触发|

## 代码示例

```lua
local part = script.Parent --获取父节点
local area = SandboxNode.new('Area', part) --创建AreaNode节点

--创建Actor实例
local actorNode = SandboxNode.new('Actor')
actorNode.Name = "my_actor"

--actorNode进入区域
area.EnterNode:connect(function(actorNode)
	print("actorNode进入区域")
end)
```