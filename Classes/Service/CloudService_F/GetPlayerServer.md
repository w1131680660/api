# GetPlayerServer

*所属类*:
* [CloudService](/Api/Classes/Service/CloudService.md)
------------------------------------------------------------------------------------------
## 描述

查询玩家所在房间(仅云服主机可用)

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|uin|[int](/Api/DataType/Number.md)||跳转玩家uinnumber|
|callback根据指定玩家的状态返回其Uin以及所在的mapid和serveridfunc|[LuaFunction](/Api/Enums/LuaFunction.md)|||
