# NavigateTo

*所属类*:
* [WorldService](/Api/Classes/GamePlay/WorldService.md)
------------------------------------------------------------------------------------------
## 描述

自动寻路至指定位置，会自动寻找最佳路径移动至指定点(接口已经废弃,请用CreatePath)

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|size|[SandboxVector3](/Api/Enums/SandboxVector3.md)||尺寸坐标|
|src|[SandboxVector3](/Api/Enums/SandboxVector3.md)||世界坐标|
|target|[SandboxVector3](/Api/Enums/SandboxVector3.md)||目标位置|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[table](/Api/DataType/Table.md)|寻路走过的block坐标数组|
