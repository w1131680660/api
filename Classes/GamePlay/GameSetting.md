# GameSetting

## 属性

|<div style="width:700px">[GameStartMode](/Api/Enums/GameStartMode.md) &emsp;<font color="dd00dd">GameStartMode</font></div>|
|:---|
|游戏开始模式|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanCunIn</font></div>|
|:---|
|游戏可否切入|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CountDown</font></div>|
|:---|
|倒数读秒|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NeedPlayerCount</font></div>|
|:---|
|最少玩家数|

|<div style="width:700px">[GameBackGroundMusic](/Api/Enums/GameBackGroundMusic.md) &emsp;<font color="dd00dd">BackgroundMusicIndex</font></div>|
|:---|
|背景音乐索引|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HideCursor</font></div>|
|:---|
|隐藏光标|

|<div style="width:700px">[ShadowDesc](/Api/Enums/ShadowDesc.md) &emsp;<font color="dd00dd">Shadow</font></div>|
|:---|
|光影开关|

|<div style="width:700px">[WaterReflectedDesc](/Api/Enums/WaterReflectedDesc.md) &emsp;<font color="dd00dd">WaterReflected</font></div>|
|:---|
|水面反射开关|

|<div style="width:700px">[ToolActiveMode](/Api/Enums/ToolActiveMode.md) &emsp;<font color="dd00dd">ToolActiveMode</font></div>|
|:---|
|道具激活方式|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LAYER1</font></div>|
|:---|
|第1层|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LAYER2</font></div>|
|:---|
|第2层|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LAYER3</font></div>|
|:---|
|第3层|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LAYER4</font></div>|
|:---|
|第4层|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LAYER5</font></div>|
|:---|
|第5层|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">SyncStream</font></div>|
|:---|
|同步流|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MusicOpen</font></div>|
|:---|
|控制地图内背景音乐开关|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">SafeSyncMode</font></div>|
|:---|
|同步安全模式|

|<div style="width:700px">[CoreUIViewRange](/Api/Enums/CoreUIViewRange.md) &emsp;<font color="dd00dd">ViewRange</font></div>|
|:---|
|视野|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">UseMnSkin</font></div>|
|:---|
|使用迷你皮肤|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Sensitivity</font></div>|
|:---|
|镜头的是否碰撞|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">AvatarPolicy</font></div>|
|:---|
|policy|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">WithoutCharacter</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CameraCollide</font></div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LoadingCustomPartTime</font></div>|
|:---|
|自定义加载条超时时间(毫秒)，0表示不开启|

|<div style="width:700px">[EMultiScenesAPI](/Api/Enums/EMultiScenesAPI.md) &emsp;<font color="dd00dd">StartScene</font></div>|
|:---|
|启动场景|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">LightActor</font></div>|
|:---|
|轻量Actor|

|<div style="width:700px">[PhysicsFrames](/Api/Enums/PhysicsFrames.md) &emsp;<font color="dd00dd">PhysicsFrames</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">PlayerIgnoreStream</font></div>|
|:---|
|player不启用流式加载|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ComputeActorInteractions</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">AvoidInteractionsSpeedFactor</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ShowAssetLoading</font></div>|
|:---|
|显示正在加载的资源|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetRunningInEditor</font>](/Api/Classes/GamePlay/GameSetting_F/GetRunningInEditor.md) ()</div>|
|:---|
|是否在编辑器中运行|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLoadingCustomPartFinished</font>](/Api/Classes/GamePlay/GameSetting_F/SetLoadingCustomPartFinished.md) ([bool](/Api/DataType/Bool.md) arg1)</div>|
|:---|
|设置loading自定义部分加载是否完成|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLoadingCustomPartLog</font>](/Api/Classes/GamePlay/GameSetting_F/SetLoadingCustomPartLog.md) ([string](/Api/DataType/String.md) arg1)</div>|
|:---|
|log|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">OpenAssetPoolGoCache</font>](/Api/Classes/GamePlay/GameSetting_F/OpenAssetPoolGoCache.md) ([bool](/Api/DataType/Bool.md) )</div>|
|:---|
||

