# NotifyPlacedBy

*所属类*：
* [BlockMaterial](/Api/Classes/Build/BlockMaterial.md)
------------------------------------------------------------------------------------------
## 描述

放置方块时，会触发一个NotifyPlacedBy通知

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|workspace|[SandboxNode_Ref](/Api/DataType/SandboxNode_Ref.md)||根节点|
|blockpos|[WCoord](/Api/DataType/WCoord.md)||方块坐标|
|player|[SandboxNode](/Api/DataType/SandboxNode.md)||玩家|
|colpoint|[Vector3](/Api/DataType/Vector3.md)||放置世界坐标|
|placeinto|[bool](/Api/DataType/Bool.md)||是否放置|
|face|[int](/Api/DataType/Number.md)||朝向|
