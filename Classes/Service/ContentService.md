# ContentService

## 属性

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RequestQueueSize</font></div>|
|:---|
|请求队列的大小|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">PreloadAsync</font>](/Api/Classes/Service/ContentService_F/PreloadAsync.md) ([LuaFunction](/Api/Enums/LuaFunction.md) func, [ReflexTuple](/Api/Enums/ReflexTuple.md) reflexTuple)</div>|
|:---|
|异步预加载|

|<div style="width:700px">[AssetFetchStatus](/Api/Enums/AssetFetchStatus.md) &emsp;[<font color="dd00dd">GetAssetFetchStatus</font>](/Api/Classes/Service/ContentService_F/GetAssetFetchStatus.md) ([string](/Api/DataType/String.md) assetid)</div>|
|:---|
|获取资源加载状态|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">GetAssetFetchStatusChangedSignal</font>](/Api/Classes/Service/ContentService_F/GetAssetFetchStatusChangedSignal.md) ([string](/Api/DataType/String.md) assetid)</div>|
|:---|
|资源加载状态变更的信号|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetAssetStatusInfo</font>](/Api/Classes/Service/ContentService_F/GetAssetStatusInfo.md) ([string](/Api/DataType/String.md) assetid)</div>|
|:---|
|获取资源加载状态信息|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyAssetFetchStatus</font>](/Api/Classes/Service/ContentService_F/NotifyAssetFetchStatus.md) ([string](/Api/DataType/String.md) assetid, [AssetFetchStatus](/Api/Enums/AssetFetchStatus.md) status)</div>|
|:---|
|资源加载状态变更时，会触发一个NotifyAssetFetchStatus通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyAssetStatusLoading</font>](/Api/Classes/Service/ContentService_F/NotifyAssetStatusLoading.md) ([string](/Api/DataType/String.md) assetid, [int](/Api/DataType/Number.md) curNum, [int](/Api/DataType/Number.md) maxNum)</div>|
|:---|
|资源加载Loading时通知|

