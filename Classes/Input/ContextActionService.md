# ContextActionService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindActivate</font>](/Api/Classes/Input/ContextActionService_F/BindActivate.md) ([int](/Api/DataType/Number.md) userInputTypeForActivate, [int](/Api/DataType/Number.md) keyCodeForActivate)</div>|
|:---|
|绑定激活|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnbindActivate</font>](/Api/Classes/Input/ContextActionService_F/UnbindActivate.md) ([int](/Api/DataType/Number.md) userInputTypeForActivate, [int](/Api/DataType/Number.md) keyCodeForActivate)</div>|
|:---|
|解绑激活|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">GetAllBoundActionInfo</font>](/Api/Classes/Input/ContextActionService_F/GetAllBoundActionInfo.md) ()</div>|
|:---|
|获取当前所有绑定的事件信息|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">GetBoundActionInfo</font>](/Api/Classes/Input/ContextActionService_F/GetBoundActionInfo.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|获取当前绑定actionName的事件信息|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetButton</font>](/Api/Classes/Input/ContextActionService_F/GetButton.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|通过绑定名称获取该按钮节点|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetCurrentLocalToolIcon</font>](/Api/Classes/Input/ContextActionService_F/GetCurrentLocalToolIcon.md) ()</div>|
|:---|
|获取当前本地tool图片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetDescription</font>](/Api/Classes/Input/ContextActionService_F/SetDescription.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) description)</div>|
|:---|
|设置描述|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetImage</font>](/Api/Classes/Input/ContextActionService_F/SetImage.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) image)</div>|
|:---|
|设置图片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetPosition</font>](/Api/Classes/Input/ContextActionService_F/SetPosition.md) ([string](/Api/DataType/String.md) actionName, [Vector2](/Api/DataType/Vector2.md) position)</div>|
|:---|
|设置位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTitle</font>](/Api/Classes/Input/ContextActionService_F/SetTitle.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) title)</div>|
|:---|
|设置标题|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindContext</font>](/Api/Classes/Input/ContextActionService_F/BindContext.md) ([string](/Api/DataType/String.md) actionname, [LuaFunction](/Api/Enums/LuaFunction.md) func, [bool](/Api/DataType/Bool.md) createTouchBtn, [ReflexVariant](/Api/Enums/ReflexVariant.md) hotkey)</div>|
|:---|
|绑定一个回调函数到指定输入上|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindContextAtPriority</font>](/Api/Classes/Input/ContextActionService_F/BindContextAtPriority.md) ([string](/Api/DataType/String.md) actionname, [LuaFunction](/Api/Enums/LuaFunction.md) func, [bool](/Api/DataType/Bool.md) createTouchBtn, [int](/Api/DataType/Number.md) priority, [ReflexVariant](/Api/Enums/ReflexVariant.md) hotkey)</div>|
|:---|
|绑定一个回调函数到指定输入上，并指定优先级|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnbindContext</font>](/Api/Classes/Input/ContextActionService_F/UnbindContext.md) ([string](/Api/DataType/String.md) actionname)</div>|
|:---|
|取消指定的用户绑定|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">UnbindAllContext</font> ()</div>|
|:---|
|移除所有的函数绑定|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">CallFunction</font>](/Api/Classes/Input/ContextActionService_F/CallFunction.md) ([string](/Api/DataType/String.md) actionName, [UserInputState](/Api/Enums/UserInputState.md) state, [SandboxNode](/Api/Classes/Base/SandboxNode.md) inputObject)</div>|
|:---|
|lua回调函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindAction</font>](/Api/Classes/Input/ContextActionService_F/BindAction.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction](/Api/Enums/LuaFunction.md) func, [int](/Api/DataType/Number.md) nActionType, [int](/Api/DataType/Number.md) nSubType)</div>|
|:---|
|这套新接口)|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindActionWithButton</font>](/Api/Classes/Input/ContextActionService_F/BindActionWithButton.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction](/Api/Enums/LuaFunction.md) func, [int](/Api/DataType/Number.md) nActionType, [int](/Api/DataType/Number.md) nSubType)</div>|
|:---|
|这套新接口)|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindActionAtPriority</font>](/Api/Classes/Input/ContextActionService_F/BindActionAtPriority.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction](/Api/Enums/LuaFunction.md) func, [int](/Api/DataType/Number.md) priority, [int](/Api/DataType/Number.md) nActionType, [int](/Api/DataType/Number.md) nSubType)</div>|
|:---|
|这套新接口)|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnbindAction</font>](/Api/Classes/Input/ContextActionService_F/UnbindAction.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|这套新接口)|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">UnbindAllActions</font> ()</div>|
|:---|
|这套新接口)|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">BoundActionChanged</font>](/Api/Classes/Input/ContextActionService_F/BoundActionChanged.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) propname, [ReflexMap](/Api/Enums/ReflexMap.md) table)</div>|
|:---|
|当绑定行为发生改变时，会触发一个BoundActionChanged时间|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">BoundActionAdded</font>](/Api/Classes/Input/ContextActionService_F/BoundActionAdded.md) ([string](/Api/DataType/String.md) actionName, [bool](/Api/DataType/Bool.md) bCreateTouchBtn, [ReflexMap](/Api/Enums/ReflexMap.md) table)</div>|
|:---|
|新增某绑定行为|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">BoundActionRemoved</font>](/Api/Classes/Input/ContextActionService_F/BoundActionRemoved.md) ([string](/Api/DataType/String.md) actionName, [ReflexMap](/Api/Enums/ReflexMap.md) table)</div>|
|:---|
|移除某绑定行为|

## 代码示例

```lua
-- 推荐使用
local ContextActionService = game:GetService("ContextActionService")
ContextActionService:BindContext("WkeydownactionName", function(actionName, inputState, inputObj)
	if inputState == Enum.UserInputState.InputBegin.Value then
		print("ContextActionService begin", actionName)
	else
		print("ContextActionService end", actionName)
	end
end, false,  Enum.KeyCode.W )

-- 即将废弃
local ContextActionService = game:GetService("ContextActionService")
local curActionName = "moveForwardAction"
local function handleMoveForward(actionName, inputState, inputObj)
	print(actionName)     -- 打印 moveForwardAction
	if inputState == Enum.UserInputState.InputBegin.Value then
		self.ForwardBackValue = 1
	else
		self.ForwardBackValue = 0
	end
	self.LocalCharacter:Move(Vector3.New(self.LeftRightValue,0,self.ForwardBackValue),true)
end
ContextActionService:BindAction(
	curActionName,
	handleMoveForward,
	Enum.ContextActionType.KeyBoard.Value,
	Enum.KeyCode.W.Value )
```