# Skeleton2D

## 属性

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">BonesDataAssetID</font></div>|
|:---|
|骨骼数据资源ID（zip/资源包）|

|<div style="width:700px">[DragonBonesSlot](/Api/Enums/DragonBonesSlot.md) &emsp;<font color="dd00dd">SlotEnum</font></div>|
|:---|
||

|<div style="width:700px">[DragonBonesSkin](/Api/Enums/DragonBonesSkin.md) &emsp;<font color="dd00dd">SkinEnum</font></div>|
|:---|
||

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Armature</font></div>|
|:---|
||

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Animation</font></div>|
|:---|
|动画名称|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Skin</font></div>|
|:---|
|皮肤名称|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Slot</font></div>|
|:---|
|插槽名称|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">DisplayOffset</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBonesDataAssetID</font>](/Api/Classes/Other/Skeleton2D_F/SetBonesDataAssetID.md) ([ModelAssetType](/Api/DataType/ModelAssetType.md) assetID, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置骨骼数据资源ID|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">LoadExtraBonesDataAsset</font>](/Api/Classes/Other/Skeleton2D_F/LoadExtraBonesDataAsset.md) ([ModelAssetType](/Api/DataType/ModelAssetType.md) assetID, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|加载额外骨骼数据资源ID（不会重复load相同资源）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ReplaceSlotDisplay</font>](/Api/Classes/Other/Skeleton2D_F/ReplaceSlotDisplay.md) ([string](/Api/DataType/String.md) , [string](/Api/DataType/String.md) , [string](/Api/DataType/String.md) , [string](/Api/DataType/String.md) , [string](/Api/DataType/String.md) , [int](/Api/DataType/Number.md) )</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSlotDisplayIndex</font>](/Api/Classes/Other/Skeleton2D_F/SetSlotDisplayIndex.md) ([string](/Api/DataType/String.md) slotName, [int](/Api/DataType/Number.md) displayIndex)</div>|
|:---|
|替换插槽|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ReplaceSkin</font>](/Api/Classes/Other/Skeleton2D_F/ReplaceSkin.md) ([string](/Api/DataType/String.md) slotName)</div>|
|:---|
|替换皮肤|

