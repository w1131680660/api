# RunService

## 属性

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LogicFPS</font></div>|
|:---|
|逻辑帧数|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">UpdateFPS</font></div>|
|:---|
|上传帧|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsClient</font>](/Api/Classes/Service/RunService_F/IsClient.md) ()</div>|
|:---|
|当前的环境是否运行在客户端上|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsServer</font>](/Api/Classes/Service/RunService_F/IsServer.md) ()</div>|
|:---|
|当前的环境是否运行在服务器上|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsStudio</font>](/Api/Classes/Service/RunService_F/IsStudio.md) ()</div>|
|:---|
|当前的环境是否运行在studio上|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsMobile</font>](/Api/Classes/Service/RunService_F/IsMobile.md) ()</div>|
|:---|
|当前的环境是否运行在手机端上|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsPC</font>](/Api/Classes/Service/RunService_F/IsPC.md) ()</div>|
|:---|
|当前的环境是否运行在电脑端上|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsRemote</font>](/Api/Classes/Service/RunService_F/IsRemote.md) ()</div>|
|:---|
|当前的环境是否远程环境|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsEdit</font>](/Api/Classes/Service/RunService_F/IsEdit.md) ()</div>|
|:---|
|当前运行环境是否为Edit（编辑)模式|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsRunMode</font>](/Api/Classes/Service/RunService_F/IsRunMode.md) ()</div>|
|:---|
|当前运行环境是否为Running模式|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Pause</font> ()</div>|
|:---|
|如果游戏在运行则暂停游戏的模拟，暂停物理运算和脚本|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">BindToRenderStep</font> ()</div>|
|:---|
|绑定RenderStep事件的Lua函数。RenderPriority为当前游戏内渲染层级，可根据需要进行插入|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">UnbindFromRenderStep</font> ()</div>|
|:---|
|解除绑定RenderStep事件的Lua函数|

|<div style="width:700px">[double](/Api/Enums/double.md) &emsp;[<font color="dd00dd">CurrentSteadyTimeStampMS</font>](/Api/Classes/Service/RunService_F/CurrentSteadyTimeStampMS.md) ()</div>|
|:---|
|获取当前时间戳，精确到毫秒。不随本地时间修改而改变。9位|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetAutoTick</font> ()</div>|
|:---|
|设置自动tick间隙|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsAutoTick</font>](/Api/Classes/Service/RunService_F/IsAutoTick.md) ()</div>|
|:---|
|是否自动tick|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">DriveTick</font> ()</div>|
|:---|
|驱动tick|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetFramePerSecond</font>](/Api/Classes/Service/RunService_F/GetFramePerSecond.md) ()</div>|
|:---|
|每秒获取帧数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetFramePerSecond</font> ()</div>|
|:---|
|设置每秒帧数值|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetMiniGameVersion</font>](/Api/Classes/Service/RunService_F/GetMiniGameVersion.md) ()</div>|
|:---|
|获取游戏端版本号|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetAppPlatformName</font>](/Api/Classes/Service/RunService_F/GetAppPlatformName.md) ()</div>|
|:---|
|获取游戏平台名称|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindToTickRegister</font>](/Api/Classes/Service/RunService_F/BindToTickRegister.md) ([string](/Api/DataType/String.md) szKey, [int](/Api/DataType/Number.md) priority, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnBindFromTickRegister</font>](/Api/Classes/Service/RunService_F/UnBindFromTickRegister.md) ([string](/Api/DataType/String.md) szKey)</div>|
|:---|
|解除绑定Tick事件的Lua函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindToRenderRegister</font>](/Api/Classes/Service/RunService_F/BindToRenderRegister.md) ([string](/Api/DataType/String.md) szKey, [int](/Api/DataType/Number.md) priority, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnBindFromRenderRegister</font>](/Api/Classes/Service/RunService_F/UnBindFromRenderRegister.md) ([string](/Api/DataType/String.md) szKey)</div>|
|:---|
|解除绑定Render事件的Lua函数|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetCurMapOwid</font>](/Api/Classes/Service/RunService_F/GetCurMapOwid.md) ()</div>|
|:---|
|获取当前地图ID|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetCurMapUpdateTimestamp</font>](/Api/Classes/Service/RunService_F/GetCurMapUpdateTimestamp.md) ()</div>|
|:---|
|获取当前地图更新时间（上传时间）|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">HeartBeat</font>](/Api/Classes/Service/RunService_F/HeartBeat.md) ([double](/Api/Enums/double.md) time)</div>|
|:---|
|心跳事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">RenderStepped</font>](/Api/Classes/Service/RunService_F/RenderStepped.md) ([double](/Api/Enums/double.md) step)</div>|
|:---|
|渲染步幅事件，每次Update触发RenderStepped事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">Stepped</font> ()</div>|
|:---|
|步幅事件，每次Tick触发Stepped事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">SystemStepped</font> ()</div>|
|:---|
|步幅事件，每次系统Tick触发SystemStepped事件|

## 代码示例

```lua
local runService = game:GetService("RunService")
local versionStr = runService:GetMiniGameVersion() --获取沙盒游戏版本号
print("Sandbox version ="..versionStr)
```