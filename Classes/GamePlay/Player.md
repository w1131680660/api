# Player

## 属性

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">Character</font></div>|
|:---|
|玩家行为|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Neutral</font></div>|
|:---|
|是否中立|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">Team</font></div>|
|:---|
|隶属的队伍|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TeamColor</font></div>|
|:---|
|隶属的队伍颜色|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">UserId</font></div>|
|:---|
|玩家的用户Id|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">Backpack</font></div>|
|:---|
|背包|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Nickname</font></div>|
|:---|
|玩家昵称|

|<div style="width:700px">[CameraModel](/Api/Enums/CameraModel.md) &emsp;<font color="dd00dd">CameraMode</font></div>|
|:---|
|玩家的相机模式（第一人称或第三人称视角）|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CameraMaxZoomDistance</font></div>|
|:---|
|玩家镜头的最大视距|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CameraMinZoomDistance</font></div>|
|:---|
|玩家镜头的最小视距|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">PlayerStateEnable</font></div>|
|:---|
|玩家状态是否显示|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">GameplayPaused</font></div>|
|:---|
|游戏暂停|

|<div style="width:700px">[DevPCMovementMode](/Api/Enums/DevPCMovementMode.md) &emsp;<font color="dd00dd">PCMovementMode</font></div>|
|:---|
|玩家在PC端移动模式|

|<div style="width:700px">[DevTouchMovementMode](/Api/Enums/DevTouchMovementMode.md) &emsp;<font color="dd00dd">TouchMovementMode</font></div>|
|:---|
|玩家在触摸屏端移动模式|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|玩家位置|

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">Rotation</font></div>|
|:---|
|玩家旋转角度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NameDisplayDistance</font></div>|
|:---|
|其他Humanoid名称对当前玩家的可见距离。设置为0时将隐藏所有名称|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TeamId</font></div>|
|:---|
|玩家的队伍Id|

|<div style="width:700px">[CoreUIViewRange](/Api/Enums/CoreUIViewRange.md) &emsp;<font color="dd00dd">ViewRange</font></div>|
|:---|
|玩家视野范围|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DefaultDie</font></div>|
|:---|
||

|<div style="width:700px">[ReflexTuple](/Api/Enums/ReflexTuple.md) &emsp;<font color="dd00dd">AvatarInfo</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">EyePos</font>](/Api/Classes/GamePlay/Player_F/EyePos.md) ([Vector3](/Api/DataType/Vector3.md) pos, [Vector3](/Api/DataType/Vector3.md) dir, [float](/Api/DataType/Number.md) dist)</div>|
|:---|
|校准碰撞视线位置|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">EyePosWithFilter</font>](/Api/Classes/GamePlay/Player_F/EyePosWithFilter.md) ([Vector3](/Api/DataType/Vector3.md) pos, [Vector3](/Api/DataType/Vector3.md) dir, [int](/Api/DataType/Number.md) filter, [float](/Api/DataType/Number.md) dist)</div>|
|:---|
|校准碰撞视线位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">EquipTool</font>](/Api/Classes/GamePlay/Player_F/EquipTool.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|给玩家装备上指定的道具|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">UnequipTools</font> ()</div>|
|:---|
|解除玩家的装备|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">DropTool</font> ()</div>|
|:---|
|丢弃装备|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">FindTool</font>](/Api/Classes/GamePlay/Player_F/FindTool.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|查询该道具是否已经装备，返回下标|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Idle</font>](/Api/Classes/GamePlay/Player_F/Idle.md) ([float](/Api/DataType/Number.md) time)</div>|
|:---|
|通常在游戏引擎将玩家定类为闲置状态的两分钟后进行触发。Time（时间）为此时点后所经历的秒数|

