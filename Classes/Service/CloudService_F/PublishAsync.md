# PublishAsync

*所属类*:
* [CloudService](/Api/Classes/Service/CloudService.md)
------------------------------------------------------------------------------------------
## 描述

房间上报分发请求（仅云服主机可用）

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|topic|[string](/Api/DataType/String.md)||消息的标识位string|
|message|[MNJsonVal](/Api/DataType/MNJsonVal.md)||消息内容any|
|serverid|[string](/Api/DataType/String.md)||目标房间的idstring|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[bool](/Api/DataType/Bool.md)|是否成功|
