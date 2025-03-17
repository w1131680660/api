# UserInputService

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TouchEnabled</font></div>|
|:---|
|当前的设备是否启用触摸屏|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">KeyboardEnabled</font></div>|
|:---|
|当前的设备是否启用键盘|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MouseEnabled</font></div>|
|:---|
|当前的设备是否启用鼠标|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AccelerometerEnabled</font></div>|
|:---|
|设备是否带启用加速器|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">GamepadEnabled</font></div>|
|:---|
|用户正在使用的设备是否启用可用的游戏手柄|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">GyroscopeEnabled</font></div>|
|:---|
|用户的设备是否启用陀螺仪|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">OnScreenKeyboardVisible</font></div>|
|:---|
|屏幕键盘当前是否在用户的屏幕上可见|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">VREnabled</font></div>|
|:---|
|用户是否正在使用头戴虚拟现实设备|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">OnScreenKeyboardPosition</font></div>|
|:---|
|屏幕键盘的位置|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MouseIconEnabled</font></div>|
|:---|
|决定Mouse的图标是否可见|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ModalEnabled</font></div>|
|:---|
|切换迷你世界Studio的移动控制是否在移动设备上隐藏|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">MouseDeltaSensitivity</font></div>|
|:---|
|缩放用户的Mouse的Delta（位置改变）输出|

|<div style="width:700px">[MouseBehavior](/Api/Enums/MouseBehavior.md) &emsp;<font color="dd00dd">MouseBehavior</font></div>|
|:---|
|用户的鼠标可以自由移动或是被锁定|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">InputBegan</font></div>|
|:---|
|开始输入|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">InputChanged</font></div>|
|:---|
|输入改变|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">InputEnded</font></div>|
|:---|
|输入结束|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">TouchStarted</font></div>|
|:---|
|触摸开始|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">TouchMoved</font></div>|
|:---|
|触摸移动|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">TouchEnded</font></div>|
|:---|
|触摸结束|

## 成员函数

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">PickObjects</font>](/Api/Classes/Input/UserInputService_F/PickObjects.md) ([float](/Api/DataType/Number.md) mouseX, [float](/Api/DataType/Number.md) mouseY, [table](/Api/DataType/Table.md) objects)</div>|
|:---|
|从给定的obj列表中，根据传入的2D屏幕坐标，拾取指定对象|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">PickObjectsEx</font>](/Api/Classes/Input/UserInputService_F/PickObjectsEx.md) ([float](/Api/DataType/Number.md) , [float](/Api/DataType/Number.md) , [table](/Api/DataType/Table.md) , [bool](/Api/DataType/Bool.md) )</div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsKeyDown</font>](/Api/Classes/Input/UserInputService_F/IsKeyDown.md) ([int](/Api/DataType/Number.md) key)</div>|
|:---|
|按键是否按下|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsRemoteSession</font>](/Api/Classes/Input/UserInputService_F/IsRemoteSession.md) ()</div>|
|:---|
|识别当前是否是远程桌面模式|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetInputObject</font>](/Api/Classes/Input/UserInputService_F/GetInputObject.md) ([UserInputType](/Api/Enums/UserInputType.md) type)</div>|
|:---|
|获取输入对象|

## 代码示例

```lua
local UserInputService = game:GetService("UserInputService")

local function inputBegan( inputObj, bGameProcessd )
	print("InputBegan")
	print( inputObj.UserInputState )   -- 0 这里都是InputBegan
	if inputObj.UserInputType == Enum.UserInputType.Keyboard.Value then
		print( "keyPressed" )
		print( inputObj.KeyCode )
	end
	if inputObj.UserInputType == Enum.UserInputType.MouseButton1.Value then
		print( "left pressed" )
		print( inputObj.Position.x ) -- 鼠标左键按下时位置
	end
end

UserInputService.InputBegan:Connect(inputBegan)
```