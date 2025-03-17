# SceneOpResult

*所属类*：
* [SandboxSceneMgrService](/Api/Classes/Other/SandboxSceneMgrService.md)
------------------------------------------------------------------------------------------
## 描述

场景操作结果通知(客户端)

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|type|[unsignedchar](/Api/DataType/unsignedchar.md)||操作类型(1:切换2:添加3:删除)|
|sceneid|[unsignedshort](/Api/DataType/unsignedshort.md)||场景id|
|result|[int](/Api/DataType/Number.md)||错误码(0:成功其他:非法错误码)|
