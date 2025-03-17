# TeleportService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Teleport</font>](/Api/Classes/GamePlay/TeleportService_F/Teleport.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) playernode, [Vector3](/Api/DataType/Vector3.md) pos)</div>|
|:---|
|地图内将玩家传送到指定位置|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">TeleportSuccess</font> ()</div>|
|:---|
|玩家传送成功触发，会触发一个TeleportSuccess通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">TeleportFail</font> ()</div>|
|:---|
|玩家传送失败，会触发一个TeleportFail通知|

## 代码示例

```lua
local TeleportService= game:GetService('TeleportService')
TeleportService:Teleport(player, Vector3.new(500, 700, 800))
```