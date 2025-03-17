# BlockService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">DropBlockAsItem</font>](/Api/Classes/Build/BlockService_F/DropBlockAsItem.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [int](/Api/DataType/Number.md) droptype, [float](/Api/DataType/Number.md) chance, [int](/Api/DataType/Number.md) useToolId)</div>|
|:---|
|将方块从道具栏丢弃|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBlock</font>](/Api/Classes/Build/BlockService_F/SetBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [int](/Api/DataType/Number.md) blockid, [int](/Api/DataType/Number.md) dir)</div>|
|:---|
|修改方块朝向|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ReplaceBlock</font>](/Api/Classes/Build/BlockService_F/ReplaceBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [int](/Api/DataType/Number.md) srcId, [int](/Api/DataType/Number.md) destId)</div>|
|:---|
|替换方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">DestroyBlock</font>](/Api/Classes/Build/BlockService_F/DestroyBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [bool](/Api/DataType/Bool.md) bDropItem)</div>|
|:---|
|销毁方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBlockAttrState</font>](/Api/Classes/Build/BlockService_F/SetBlockAttrState.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [int](/Api/DataType/Number.md) blockid, [int](/Api/DataType/Number.md) attrType, [bool](/Api/DataType/Bool.md) bActive)</div>|
|:---|
|设置方块属性状态|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetFunctionBlockTrigger</font>](/Api/Classes/Build/BlockService_F/SetFunctionBlockTrigger.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) pos, [bool](/Api/DataType/Bool.md) bActive)</div>|
|:---|
|设置功能方块触发器（区域笔刷）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AreaFillBlock</font>](/Api/Classes/Build/BlockService_F/AreaFillBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) areaNode, [int](/Api/DataType/Number.md) blockid)</div>|
|:---|
|区域内填充方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AreaClearBlock</font>](/Api/Classes/Build/BlockService_F/AreaClearBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) areaNode)</div>|
|:---|
|区域内删除方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AreaReplaceBlock</font>](/Api/Classes/Build/BlockService_F/AreaReplaceBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) areaNode, [int](/Api/DataType/Number.md) srcId, [int](/Api/DataType/Number.md) destId)</div>|
|:---|
|区域替换方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AreaCopyBlock</font>](/Api/Classes/Build/BlockService_F/AreaCopyBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) areaNode, [SandboxVector3](/Api/Enums/SandboxVector3.md) destPos)</div>|
|:---|
|区域拷贝方块|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBlockSettingAttState</font>](/Api/Classes/Build/BlockService_F/SetBlockSettingAttState.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [int](/Api/DataType/Number.md) blockid, [int](/Api/DataType/Number.md) attr, [bool](/Api/DataType/Bool.md) bOpen)</div>|
|:---|
|设置方块的属性设置状态|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetRayBlock</font>](/Api/Classes/Build/BlockService_F/GetRayBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3, [int](/Api/DataType/Number.md) face, [float](/Api/DataType/Number.md) distance)</div>|
|:---|
|获取方块光线|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsSolidBlock</font>](/Api/Classes/Build/BlockService_F/IsSolidBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|是否固体方块|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsLiquidBlock</font>](/Api/Classes/Build/BlockService_F/IsLiquidBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|是否液体方块|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsAirBlock</font>](/Api/Classes/Build/BlockService_F/IsAirBlock.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|是否空气方块|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetBlockData</font>](/Api/Classes/Build/BlockService_F/GetBlockData.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|获取方块朝向数据|

|<div style="width:700px">[SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) &emsp;[<font color="dd00dd">GetBlockMaterial</font>](/Api/Classes/Build/BlockService_F/GetBlockMaterial.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|获取方块材质|

|<div style="width:700px">[SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) &emsp;[<font color="dd00dd">GetBlockNode</font>](/Api/Classes/Build/BlockService_F/GetBlockNode.md) ([SandboxNode_Ref](/Api/Enums/SandboxNode_Ref.md) workspace, [SandboxVector3](/Api/Enums/SandboxVector3.md) vector3)</div>|
|:---|
|获取方块节点|

