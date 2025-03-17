# CloudService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetValue</font>](/Api/Classes/Service/CloudService_F/SetValue.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) value)</div>|
|:---|
|设置同步value值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetValue</font>](/Api/Classes/Service/CloudService_F/GetValue.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name)</div>|
|:---|
|获取同步value值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetValueAsync</font>](/Api/Classes/Service/CloudService_F/SetValueAsync.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) value, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|设置异步value值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetValueAsync</font>](/Api/Classes/Service/CloudService_F/GetValueAsync.md) ([string](/Api/DataType/String.md) key, [string](/Api/DataType/String.md) name, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取异步value值|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetOrderDataCloud</font>](/Api/Classes/Service/CloudService_F/GetOrderDataCloud.md) ([string](/Api/DataType/String.md) tableName)</div>|
|:---|
|获取订单数据云节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTable</font>](/Api/Classes/Service/CloudService_F/SetTable.md) ([string](/Api/DataType/String.md) key, [LuaTable](/Api/DataType/LuaTable.md) value)</div>|
|:---|
|设置同步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetTable</font>](/Api/Classes/Service/CloudService_F/GetTable.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取同步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTableAsync</font>](/Api/Classes/Service/CloudService_F/SetTableAsync.md) ([string](/Api/DataType/String.md) key, [LuaTable](/Api/DataType/LuaTable.md) value, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|设置异步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetTableAsync</font>](/Api/Classes/Service/CloudService_F/GetTableAsync.md) ([string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取异步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetTableOrEmpty</font>](/Api/Classes/Service/CloudService_F/GetTableOrEmpty.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取同步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetTableOrEmptyAsync</font>](/Api/Classes/Service/CloudService_F/GetTableOrEmptyAsync.md) ([string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取异步table值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveKey</font>](/Api/Classes/Service/CloudService_F/RemoveKey.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|同步移除key|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveKeyAsync</font>](/Api/Classes/Service/CloudService_F/RemoveKeyAsync.md) ([string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取移除key|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">PublishAsync</font>](/Api/Classes/Service/CloudService_F/PublishAsync.md) ([string](/Api/DataType/String.md) topic, [MNJsonVal](/Api/DataType/MNJsonVal.md) message)</div>|
|:---|
|房间上报分发请求（仅云服主机可用）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">PublishAsync</font>](/Api/Classes/Service/CloudService_F/PublishAsync.md) ([string](/Api/DataType/String.md) topic, [MNJsonVal](/Api/DataType/MNJsonVal.md) message, [string](/Api/DataType/String.md) serverid)</div>|
|:---|
|房间上报分发请求（仅云服主机可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SubscribeAsync</font>](/Api/Classes/Service/CloudService_F/SubscribeAsync.md) ([string](/Api/DataType/String.md) topic, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|房间监听消息（仅云服主机可用）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">TeleportToMap</font>](/Api/Classes/Service/CloudService_F/TeleportToMap.md) ([longlong](/Api/Enums/longlong.md) mapid, [int](/Api/DataType/Number.md) uin, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData)</div>|
|:---|
|跳转到地图|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">TeleportToMap</font>](/Api/Classes/Service/CloudService_F/TeleportToMap.md) ([longlong](/Api/Enums/longlong.md) mapid, [int](/Api/DataType/Number.md) uin, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData, [ReflexMap](/Api/Enums/ReflexMap.md) reportData)</div>|
|:---|
|跳转到地图|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">TeleportToMap</font>](/Api/Classes/Service/CloudService_F/TeleportToMap.md) ([longlong](/Api/Enums/longlong.md) mapid, [int](/Api/DataType/Number.md) uin, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData, [ReflexMap](/Api/Enums/ReflexMap.md) reportData, [bool](/Api/DataType/Bool.md) false跳过确认框)</div>|
|:---|
|跳转到地图|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">TeleportToServer</font>](/Api/Classes/Service/CloudService_F/TeleportToServer.md) ([string](/Api/DataType/String.md) serverid, [int](/Api/DataType/Number.md) uin, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData)</div>|
|:---|
|跳转到房间|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">TeleportToServer</font>](/Api/Classes/Service/CloudService_F/TeleportToServer.md) ([string](/Api/DataType/String.md) serverid, [int](/Api/DataType/Number.md) uin, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData, [ReflexMap](/Api/Enums/ReflexMap.md) reportData)</div>|
|:---|
|跳转到房间|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetPlayerServer</font>](/Api/Classes/Service/CloudService_F/GetPlayerServer.md) ([int](/Api/DataType/Number.md) uin, [LuaFunction](/Api/Enums/LuaFunction.md) callback根据指定玩家的状态返回其Uin以及所在的mapid和serveridfunc)</div>|
|:---|
|查询玩家所在房间(仅云服主机可用)|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">ReserveServer</font>](/Api/Classes/Service/CloudService_F/ReserveServer.md) ([int](/Api/DataType/Number.md) uin, [longlong](/Api/Enums/longlong.md) mapid, [MNJsonVal](/Api/DataType/MNJsonVal.md) serverData)</div>|
|:---|
|开启并跳转到新房间|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">ReserveServer</font>](/Api/Classes/Service/CloudService_F/ReserveServer.md) ([int](/Api/DataType/Number.md) uin, [longlong](/Api/Enums/longlong.md) mapid, [MNJsonVal](/Api/DataType/MNJsonVal.md) serverData, [MNJsonVal](/Api/DataType/MNJsonVal.md) teleportData, [ReflexMap](/Api/Enums/ReflexMap.md) reportData)</div>|
|:---|
|开启并跳转到新房间|

|<div style="width:700px">[MNJsonVal](/Api/DataType/MNJsonVal.md) &emsp;[<font color="dd00dd">GetServerRoomType</font>](/Api/Classes/Service/CloudService_F/GetServerRoomType.md) ()</div>|
|:---|
|any|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetServerID</font>](/Api/Classes/Service/CloudService_F/GetServerID.md) ()</div>|
|:---|
|获取服务ID|

|<div style="width:700px">[MNJsonVal](/Api/DataType/MNJsonVal.md) &emsp;[<font color="dd00dd">GetPlayerTeleportInfo</font>](/Api/Classes/Service/CloudService_F/GetPlayerTeleportInfo.md) ()</div>|
|:---|
||

|<div style="width:700px">[MNJsonVal](/Api/DataType/MNJsonVal.md) &emsp;[<font color="dd00dd">GetServerPlayerTeleportInfo</font>](/Api/Classes/Service/CloudService_F/GetServerPlayerTeleportInfo.md) ([int](/Api/DataType/Number.md) uin)</div>|
|:---|
|获取玩家进入房间时伴随的自定义数据（如果有）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetForbidJoin</font>](/Api/Classes/Service/CloudService_F/SetForbidJoin.md) ()</div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">SetDataListByKey</font>](/Api/Classes/Service/CloudService_F/SetDataListByKey.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key, [LuaArguments](/Api/Enums/LuaArguments.md) value)</div>|
|:---|
|存储带表名name得kv|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">SetDataListByKeyAsync</font>](/Api/Classes/Service/CloudService_F/SetDataListByKeyAsync.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key, [LuaArguments](/Api/Enums/LuaArguments.md) value, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|存储带表名name得kv|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetDataListByKey</font>](/Api/Classes/Service/CloudService_F/GetDataListByKey.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key)</div>|
|:---|
|获取表名name，键值k存储得值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetDataListByKeyAsync</font>](/Api/Classes/Service/CloudService_F/GetDataListByKeyAsync.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|获取表名name，键值k存储得值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">RemoveDataListByKey</font>](/Api/Classes/Service/CloudService_F/RemoveDataListByKey.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key)</div>|
|:---|
|移除表名name，键值k存储得值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">RemoveDataListByKeyAsync</font>](/Api/Classes/Service/CloudService_F/RemoveDataListByKeyAsync.md) ([string](/Api/DataType/String.md) name, [string](/Api/DataType/String.md) key, [LuaFunction](/Api/Enums/LuaFunction.md) func)</div>|
|:---|
|移除表名name，键值k存储得值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">ClearDataList</font>](/Api/Classes/Service/CloudService_F/ClearDataList.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|的全部kv|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">ClearDataListAsync</font>](/Api/Classes/Service/CloudService_F/ClearDataListAsync.md) ([string](/Api/DataType/String.md) name, [LuaFunction](/Api/Enums/LuaFunction.md) arg2)</div>|
|:---|
|的全部kv|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetCenterServerAsync</font>](/Api/Classes/Service/CloudService_F/GetCenterServerAsync.md) ([string](/Api/DataType/String.md) string, [string](/Api/DataType/String.md) string, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|查询/开启标识为key的中心服，回调函数返回serverid（房间ID）,同key中心服不会开启两个，除非上一个已关闭|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetCenterServerKey</font>](/Api/Classes/Service/CloudService_F/GetCenterServerKey.md) ()</div>|
|:---|
|获取当前中心服的标识key，如果不是中心服，返回""|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ShutdownServer</font>](/Api/Classes/Service/CloudService_F/ShutdownServer.md) ([string](/Api/DataType/String.md) string)</div>|
|:---|
|关闭当前云服（任何云服），要确保玩家正确下线（一般房间云服）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SendMessage</font>](/Api/Classes/Service/CloudService_F/SendMessage.md) ([LuaTable](/Api/DataType/LuaTable.md) vector, [ReflexTuple](/Api/Enums/ReflexTuple.md) arg2)</div>|
|:---|
|向roomids数组指定的房间发送tcp直连消息|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyOnMessage</font>](/Api/Classes/Service/CloudService_F/NotifyOnMessage.md) ([string](/Api/DataType/String.md) string, [ReflexTuple](/Api/Enums/ReflexTuple.md) ReflexTuple)</div>|
|:---|
|接收所有tcp直连消息的事件|

