# TeleportToServer

*所属类*:
* [CloudService](/Api/Classes/Service/CloudService.md)
------------------------------------------------------------------------------------------
## 描述

跳转到房间

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|serverid|[string](/Api/DataType/String.md)||跳转目标房间的房间idstring|
|uin|[int](/Api/DataType/Number.md)||跳转玩家uinnumber|
|teleportData|[MNJsonVal](/Api/DataType/MNJsonVal.md)||自定义的跳转信息any|
|reportData|[ReflexMap](/Api/Enums/ReflexMap.md)||埋点相关信息{maptype，mapname}any|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[bool](/Api/DataType/Bool.md)|是否成功|
