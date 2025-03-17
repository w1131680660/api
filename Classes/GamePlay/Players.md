# Players

## 属性

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">LocalPlayer</font></div>|
|:---|
|是一个只读属性，指的是其客户端正在运行体验的玩家|

## 成员函数

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetPlayerByUserId</font>](/Api/Classes/GamePlay/Players_F/GetPlayerByUserId.md) ([int](/Api/DataType/Number.md) userid)</div>|
|:---|
|在Players中搜索每个玩家，以查找其player.UserId与给定UserId匹配的玩家|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetPlayers</font>](/Api/Classes/GamePlay/Players_F/GetPlayers.md) ()</div>|
|:---|
|返回当前连接的所有玩家的表|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">HideTouchUI</font> ()</div>|
|:---|
|隐藏触摸UI|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">HideJump</font> ()</div>|
|:---|
|隐藏跳跃|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">HideRocker</font> ()</div>|
|:---|
|隐藏摇杆|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SendFriendApply</font>](/Api/Classes/GamePlay/Players_F/SendFriendApply.md) ([int](/Api/DataType/Number.md) nUin1, [int](/Api/DataType/Number.md) nUin2)</div>|
|:---|
|申请好友|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">HasFriend</font>](/Api/Classes/GamePlay/Players_F/HasFriend.md) ([int](/Api/DataType/Number.md) nUin1, [int](/Api/DataType/Number.md) nUin2, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|判断好友|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerAdded</font>](/Api/Classes/GamePlay/Players_F/PlayerAdded.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) player)</div>|
|:---|
|避免分发事件时还没执行脚本监听代码。建议放于StartPlayer.StarterPlayerScripts下的脚本节点的头部。|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerRemoving</font>](/Api/Classes/GamePlay/Players_F/PlayerRemoving.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) player)</div>|
|:---|
|玩家移除事件，在玩家离开游戏之前立即触发。由于它在实际移除Player之前激发，因此此事件对于需要存储玩家数据非常有用|

## 代码示例

```lua
local players = game:GetService("Players")
local playerlist = players:GetPlayers()
for i, v in ipairs( playerlist ) do
	print( v.ClassType )
end
```