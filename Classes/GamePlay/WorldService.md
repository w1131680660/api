# WorldService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">PrintLog</font>](/Api/Classes/GamePlay/WorldService_F/PrintLog.md) ([string](/Api/DataType/String.md) szLog)</div>|
|:---|
|打印日志|

|<div style="width:700px">[ReflexTuple](/Api/Enums/ReflexTuple.md) &emsp;[<font color="dd00dd">GetRangeXZ</font>](/Api/Classes/GamePlay/WorldService_F/GetRangeXZ.md) ()</div>|
|:---|
|的坐标|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetUIScale</font>](/Api/Classes/GamePlay/WorldService_F/GetUIScale.md) ()</div>|
|:---|
|获取UI布局的缩放尺寸|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">RaycastClosest</font>](/Api/Classes/GamePlay/WorldService_F/RaycastClosest.md) ([SandboxVector3](/Api/Enums/SandboxVector3.md) origin, [SandboxVector3](/Api/Enums/SandboxVector3.md) unitDir, [float](/Api/DataType/Number.md) distance, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|射线段检测，返回最近的碰撞物|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">RaycastAll</font>](/Api/Classes/GamePlay/WorldService_F/RaycastAll.md) ([SandboxVector3](/Api/Enums/SandboxVector3.md) origin, [SandboxVector3](/Api/Enums/SandboxVector3.md) unitDir, [float](/Api/DataType/Number.md) distance, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|射线段检测，返回所有碰撞物，最多128个|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">SweepBoxAll</font>](/Api/Classes/GamePlay/WorldService_F/SweepBoxAll.md) ([SandboxVector3](/Api/Enums/SandboxVector3.md) center, [SandboxVector3](/Api/Enums/SandboxVector3.md) shape, [SandboxVector3](/Api/Enums/SandboxVector3.md) direction, [SandboxVector3](/Api/Enums/SandboxVector3.md) angle, [float](/Api/DataType/Number.md) distance, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|扫描全部|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">SweepCapsuleAll</font>](/Api/Classes/GamePlay/WorldService_F/SweepCapsuleAll.md) ([float](/Api/DataType/Number.md) radius, [SandboxVector3](/Api/Enums/SandboxVector3.md) p0, [SandboxVector3](/Api/Enums/SandboxVector3.md) p1, [SandboxVector3](/Api/Enums/SandboxVector3.md) dir, [float](/Api/DataType/Number.md) distance, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|扫描胶囊全部|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">SweepSphereAll</font>](/Api/Classes/GamePlay/WorldService_F/SweepSphereAll.md) ([float](/Api/DataType/Number.md) radius, [SandboxVector3](/Api/Enums/SandboxVector3.md) center, [SandboxVector3](/Api/Enums/SandboxVector3.md) direction, [float](/Api/DataType/Number.md) distance, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|扫描球全部|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">OverlapBox</font>](/Api/Classes/GamePlay/WorldService_F/OverlapBox.md) ([SandboxVector3](/Api/Enums/SandboxVector3.md) shape, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [SandboxVector3](/Api/Enums/SandboxVector3.md) angle, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|重叠框|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">OverlapCapsule</font>](/Api/Classes/GamePlay/WorldService_F/OverlapCapsule.md) ([float](/Api/DataType/Number.md) radius, [SandboxVector3](/Api/Enums/SandboxVector3.md) p0, [SandboxVector3](/Api/Enums/SandboxVector3.md) p1, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|重叠胶囊|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">OverlapSphere</font>](/Api/Classes/GamePlay/WorldService_F/OverlapSphere.md) ([float](/Api/DataType/Number.md) radius, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [bool](/Api/DataType/Bool.md) isIgnoreTrigger, [table](/Api/DataType/Table.md) filterGroup)</div>|
|:---|
|重叠球体|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMainFrameShow</font>](/Api/Classes/GamePlay/WorldService_F/SetMainFrameShow.md) ([bool](/Api/DataType/Bool.md) isShow)</div>|
|:---|
|用于隐藏显示游戏内置UI|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetUISize</font>](/Api/Classes/GamePlay/WorldService_F/GetUISize.md) ()</div>|
|:---|
|获取UI布局的尺寸|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">EmitMiniGameESCKey</font>](/Api/Classes/GamePlay/WorldService_F/EmitMiniGameESCKey.md) ()</div>|
|:---|
|流程|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">TeleportPlayer</font>](/Api/Classes/GamePlay/WorldService_F/TeleportPlayer.md) ([int](/Api/DataType/Number.md) mapid)</div>|
|:---|
|传送玩家到地图|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetActorHp</font>](/Api/Classes/GamePlay/WorldService_F/SetActorHp.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) actornode, [float](/Api/DataType/Number.md) hp)</div>|
|:---|
|设置生物血量|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetActorMotion</font>](/Api/Classes/GamePlay/WorldService_F/SetActorMotion.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) actornode, [Vector3](/Api/DataType/Vector3.md) motion)</div>|
|:---|
|设置生物动作|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AttackTarget</font>](/Api/Classes/GamePlay/WorldService_F/AttackTarget.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) actornode)</div>|
|:---|
|设置攻击目标|

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;[<font color="dd00dd">NavigateTo</font>](/Api/Classes/GamePlay/WorldService_F/NavigateTo.md) ([SandboxVector3](/Api/Enums/SandboxVector3.md) size, [SandboxVector3](/Api/Enums/SandboxVector3.md) src, [SandboxVector3](/Api/Enums/SandboxVector3.md) target)</div>|
|:---|
|自动寻路至指定位置，会自动寻找最佳路径移动至指定点(接口已经废弃,请用CreatePath)|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">CreatePath</font>](/Api/Classes/GamePlay/WorldService_F/CreatePath.md) ([ReflexMap](/Api/Enums/ReflexMap.md) Radius,Heigh,StepOffset,SlopLimit,CollideGroupID)</div>|
|:---|
|创建一个路径基于想要模拟的actor的参数.|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetSceneId</font>](/Api/Classes/GamePlay/WorldService_F/SetSceneId.md) ([int](/Api/DataType/Number.md) id)</div>|
|:---|
|设置当前worldservice的world的SceneId|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetSceneId</font>](/Api/Classes/GamePlay/WorldService_F/GetSceneId.md) ()</div>|
|:---|
|获取当前worldservice的world的SceneId|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">DoGmCmd</font>](/Api/Classes/GamePlay/WorldService_F/DoGmCmd.md) ([string](/Api/DataType/String.md) )</div>|
|:---|
||

