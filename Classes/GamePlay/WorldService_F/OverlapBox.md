# OverlapBox

*所属类*:
* [WorldService](/Api/Classes/GamePlay/WorldService.md)
------------------------------------------------------------------------------------------
## 描述

重叠框

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|shape|[SandboxVector3](/Api/Enums/SandboxVector3.md)||长、宽、高的一半大小|
|pos|[SandboxVector3](/Api/Enums/SandboxVector3.md)||中心点的世界坐标|
|angle|[SandboxVector3](/Api/Enums/SandboxVector3.md)||朝向角度|
|isIgnoreTrigger|[bool](/Api/DataType/Bool.md)||是否忽略trigger类型|
|filterGroup|[table](/Api/DataType/Table.md)||过滤组，{1，2，3}含有的数字组会被查询|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[ReflexMap](/Api/Enums/ReflexMap.md)|{isHit ,normal ,position , distance ,obj}数组|
