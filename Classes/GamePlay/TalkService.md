# TalkService

*继承自*：
* [Service](/Api/Classes/Service/Service.md)

## 描述

一种处理体验式文本聊天的服务。TalkService处理各种与文本聊天相关的任务，如管理频道、装饰消息、过滤文本、创建命令和开发自定义聊天界面。

## 函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">GetMessage</font>](/Api/Classes/GamePlay/TalkService_F/GetMessage.md) ([int](/Api/DataType/Number.md) id, [LuaFunction](/Api/DataType/LuaFunction.md) callback)</div>|
|:---|
|获取聊天信息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SendMessage</font>](/Api/Classes/GamePlay/TalkService_F/SendMessage.md) ([int](/Api/DataType/Number.md) id, [string](/Api/DataType/String.md) msg, [LuaFunction](/Api/DataType/LuaFunction.md) callback)</div>|
|:---|
|发送聊天信息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCallBack</font>](/Api/Classes/GamePlay/TalkService_F/SetCallBack.md) ([int](/Api/DataType/Number.md) key, [LuaFunction](/Api/DataType/LuaFunction.md) callback)</div>|
|:---|
|设置回调函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveCallBack</font>](/Api/Classes/GamePlay/TalkService_F/RemoveCallBack.md) ([int](/Api/DataType/Number.md) key)</div>|
|:---|
|移除回调函数|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BindNPCId</font>](/Api/Classes/GamePlay/TalkService_F/BindNPCId.md) ([int](/Api/DataType/Number.md) sandboxNodeId)</div>|
|:---|
|绑定NPC|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UnBindNPCId</font>](/Api/Classes/GamePlay/TalkService_F/UnBindNPCId.md) ([int](/Api/DataType/Number.md) sandboxNodeId)</div>|
|:---|
|解绑NPC|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">QueryNPCId</font>](/Api/Classes/GamePlay/TalkService_F/QueryNPCId.md) ([int](/Api/DataType/Number.md) sandboxNodeId)</div>|
|:---|
|查询该沙盒节点绑定的NPCId|

