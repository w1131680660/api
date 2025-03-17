# NotifyDestroyedBy

*所属类*：
* [BlockMaterial](/Api/Classes/Build/BlockMaterial.md)
------------------------------------------------------------------------------------------
## 描述

销毁方块时，会触发一个NotifyDestroyedBy通知

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|workspace|[SandboxNode_Ref](/Api/DataType/SandboxNode_Ref.md)||根节点|
|blockpos|[WCoord](/Api/DataType/WCoord.md)||方块坐标|
|blockdata|[int](/Api/DataType/Number.md)||方块数据|
|destroytype|[int](/Api/DataType/Number.md)||销毁类型|
|bywho|[SandboxNode](/Api/DataType/SandboxNode.md)||销毁的生物|
