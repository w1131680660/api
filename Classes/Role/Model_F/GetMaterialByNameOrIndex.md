# GetMaterialByNameOrIndex

*所属类*:
* [Model](/Api/Classes/Role/Model.md)
------------------------------------------------------------------------------------------
## 描述

获取材质节点

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|findKey|[string](/Api/DataType/String.md)||名称或者序号字符串|
|byName|[bool](/Api/DataType/Bool.md)||findKey是否为名称|
|isSkinMeshRender|[bool](/Api/DataType/Bool.md)||是否查找SkinMeshRender|
|materialIndex|[int](/Api/DataType/Number.md)||下标|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[SandboxNode](/Api/Classes/Base/SandboxNode.md)|材质对象|
