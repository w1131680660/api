# GetCenterServerAsync

*所属类*:
* [CloudService](/Api/Classes/Service/CloudService.md)
------------------------------------------------------------------------------------------
## 描述

查询/开启标识为key的中心服，回调函数返回serverid（房间ID）,同key中心服不会开启两个，除非上一个已关闭

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|string|[string](/Api/DataType/String.md)||标识的中心服|
|string|[string](/Api/DataType/String.md)||可选的mapid指定以另一个地图id开启中心服，但要求目标地图与当前地图同属一个AppID|
|callback|[LuaFunction](/Api/Enums/LuaFunction.md)||回调函数返回roomid（房间ID）|
