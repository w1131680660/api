# Tool

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanBeDropped</font></div>|
|:---|
|可否丢弃道具，默认不可以丢弃|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Enabled</font></div>|
|:---|
|决定道具能否被使用，默认可以使用|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GripPos</font></div>|
|:---|
|夹点位置|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GripEuler</font></div>|
|:---|
|夹点的欧拉|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">ToolTip</font></div>|
|:---|
|道具提示信息|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">TextureId</font></div>|
|:---|
|默认快捷栏界面，显示的图标资源|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ActivationOnly</font></div>|
|:---|
|仅激活|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Activate</font>](/Api/Classes/GamePlay/Tool_F/Activate.md) ()</div>|
|:---|
|已装备的的工具，模拟点击使用，会触发Activated事件。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Deactivate</font>](/Api/Classes/GamePlay/Tool_F/Deactivate.md) ()</div>|
|:---|
|模拟工具的结束使用。|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">Activated</font> ()</div>|
|:---|
|玩家已装备工具，点击鼠标左键时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">Deactivated</font> ()</div>|
|:---|
|当鼠标左键松开时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">Equipped</font> ()</div>|
|:---|
|当装备道具时触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">Unequipped</font> ()</div>|
|:---|
|当卸载道具时触发。|

## 代码示例

```lua
 --以下示例是使用LocalPlayer的EquipTool，UnequipTools接口，装备指定Tool和卸下Tool 的示例。将其放到Tool下的Script节点里，按X装备该Tool，按Z卸下当前的装备（不管是不是该Tool节点）
 local tool = script.Parent
 local playersService = game:GetService("Players")
 local localPlayer = playersService.LocalPlayer

 local ContextActionService = game:GetService("ContextActionService")

 local function testEquipTool(actionName, inputState, inputObj)
	 if inputState == Enum.UserInputState.InputBegin.Value then
		 localPlayer:EquipTool( tool )
	 end
 end
 ContextActionService:BindAction(
	 "testEquipTool",
	 testEquipTool,
	 Enum.ContextActionType.KeyBoard.Value,
	 string.byte('X') )

 local function testUnequipTool(actionName, inputState, inputObj)
	 if inputState == Enum.UserInputState.InputBegin.Value then
		 localPlayer:UnequipTools()
	 end
 end

 ContextActionService:BindAction(
	 "testUnequipTool",
	 testUnequipTool,
	 Enum.ContextActionType.KeyBoard.Value,
	 string.byte('Z') )
 ```