# DynamicSceneOpResultServer

*所属类*:
* [SandboxSceneMgrService](/Api/Classes/Service/SandboxSceneMgrService.md)
------------------------------------------------------------------------------------------
## 描述

动态场景操作结果通知(服务端)

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|type|[unsignedchar](/Api/Enums/unsignedchar.md)||操作类型(1:切换2:添加3:删除)|
|sceneid|[unsignedshort](/Api/Enums/unsignedshort.md)||场景id|
|result|[int](/Api/DataType/Number.md)||错误码(0:成功其他:非法错误码)|
|uid|[int](/Api/DataType/Number.md)||操作用户uid(仅type==切换时有效)|
