# Animator

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Pause</font></div>|
|:---|
|是否暂停|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">SkeletonAsset</font></div>|
|:---|
|骨骼资源|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">ControllerAsset</font></div>|
|:---|
|动画控制器资源|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Speed</font></div>|
|:---|
||

|<div style="width:700px">[uint32_t](/Api/Enums/uint32_t.md) &emsp;<font color="dd00dd">SkipSampleRate</font></div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CullingMode</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FixedTickTime</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ModelWaitForLoaded</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的资源|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Classes/Animation/Animator_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetControllerAsset</font>](/Api/Classes/Animation/Animator_F/SetControllerAsset.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|设置动画控制器资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateControllerAsset</font>](/Api/Classes/Animation/Animator_F/UpdateControllerAsset.md) ([AssetResType](/Api/Enums/AssetResType.md) restype, [string](/Api/DataType/String.md) url)</div>|
|:---|
|更新动画控制器资源|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">NewController</font>](/Api/Classes/Animation/Animator_F/NewController.md) ([int](/Api/DataType/Number.md) type)</div>|
|:---|
|新建一个默认的状态机数据：1-AnimatorControllerData；2-AnimatorOverrideController；|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetControllerAsset</font>](/Api/Classes/Animation/Animator_F/GetControllerAsset.md) ()</div>|
|:---|
|获取动画控制器资源|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSkeleton</font>](/Api/Classes/Animation/Animator_F/GetSkeleton.md) ()</div>|
|:---|
|获取当前的骨骼资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSkeleton</font>](/Api/Classes/Animation/Animator_F/SetSkeleton.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|设置骨骼资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateSkeleton</font>](/Api/Classes/Animation/Animator_F/UpdateSkeleton.md) ([AssetResType](/Api/Enums/AssetResType.md) restype, [string](/Api/DataType/String.md) url)</div>|
|:---|
|更新骨骼资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Play</font>](/Api/Classes/Animation/Animator_F/Play.md) ([string](/Api/DataType/String.md) name, [int](/Api/DataType/Number.md) layer, [float](/Api/DataType/Number.md) normalized)</div>|
|:---|
|播放一个state|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">CrossFade</font>](/Api/Classes/Animation/Animator_F/CrossFade.md) ([string](/Api/DataType/String.md) stateName, [int](/Api/DataType/Number.md) layer, [float](/Api/DataType/Number.md) transitionTotal, [float](/Api/DataType/Number.md) transitionOffset)</div>|
|:---|
|渐变动画：淡入淡出|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetFloat</font>](/Api/Classes/Animation/Animator_F/SetFloat.md) ([string](/Api/DataType/String.md) key, [float](/Api/DataType/Number.md) value)</div>|
|:---|
|设置animator属性的浮点数数据类型KV值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetInt</font>](/Api/Classes/Animation/Animator_F/SetInt.md) ([string](/Api/DataType/String.md) key, [int](/Api/DataType/Number.md) value)</div>|
|:---|
|设置animator属性的整数数据类型KV值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBool</font>](/Api/Classes/Animation/Animator_F/SetBool.md) ([string](/Api/DataType/String.md) key, [bool](/Api/DataType/Bool.md) value)</div>|
|:---|
|设置animator属性的布尔数据类型KV值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTrigger</font>](/Api/Classes/Animation/Animator_F/SetTrigger.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|设置触发器|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetFloat</font>](/Api/Classes/Animation/Animator_F/GetFloat.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取animator属性的浮点数数据类型KV值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetInt</font>](/Api/Classes/Animation/Animator_F/GetInt.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取animator属性的整数数据类型KV值|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetBool</font>](/Api/Classes/Animation/Animator_F/GetBool.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取animator属性的布尔数据类型KV值|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetTrigger</font>](/Api/Classes/Animation/Animator_F/GetTrigger.md) ([string](/Api/DataType/String.md) key)</div>|
|:---|
|获取触发器|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetLayerCount</font>](/Api/Classes/Animation/Animator_F/GetLayerCount.md) ()</div>|
|:---|
|获取当前layer的个数|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetLayerByIndex</font>](/Api/Classes/Animation/Animator_F/GetLayerByIndex.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|按照index获取层级节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLayerWeight</font>](/Api/Classes/Animation/Animator_F/SetLayerWeight.md) ([int](/Api/DataType/Number.md) layer, [float](/Api/DataType/Number.md) value)</div>|
|:---|
|设置layer层级权重|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetLayerWeight</font>](/Api/Classes/Animation/Animator_F/GetLayerWeight.md) ([int](/Api/DataType/Number.md) layer)</div>|
|:---|
|获取layer层级权重|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBoneTransform</font>](/Api/Classes/Animation/Animator_F/SetBoneTransform.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) targetBoneNode, [SandboxNode](/Api/Classes/Base/SandboxNode.md) baseBoneNode, [Vector3](/Api/DataType/Vector3.md) translate, [Vector3](/Api/DataType/Vector3.md) rotation, [Vector3](/Api/DataType/Vector3.md) scale)</div>|
|:---|
|设置骨骼变换|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBoneModelSpaceRotate</font>](/Api/Classes/Animation/Animator_F/SetBoneModelSpaceRotate.md) ([string](/Api/DataType/String.md) boneName, [float](/Api/DataType/Number.md) pitch, [float](/Api/DataType/Number.md) yaw, [float](/Api/DataType/Number.md) roll)</div>|
|:---|
|设置骨骼模型空间旋转|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetStatePlayedTime</font>](/Api/Classes/Animation/Animator_F/GetStatePlayedTime.md) ([string](/Api/DataType/String.md) stateFullName)</div>|
|:---|
|获取状态的PlayedTime|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetCurrentStatePlayedTime</font>](/Api/Classes/Animation/Animator_F/GetCurrentStatePlayedTime.md) ([int](/Api/DataType/Number.md) layerIdx)</div>|
|:---|
|获取当前层级正在播放的状态的PlayedTime|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetStatePauseAtNormlizedTime</font>](/Api/Classes/Animation/Animator_F/SetStatePauseAtNormlizedTime.md) ([string](/Api/DataType/String.md) , [bool](/Api/DataType/Bool.md) , [float](/Api/DataType/Number.md) )</div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">EventNotify</font>](/Api/Classes/Animation/Animator_F/EventNotify.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) statedata, [constchar*](/Api/Enums/constchar*.md) name, [int](/Api/DataType/Number.md) layerIndex, [StateMachineMessage](/Api/Enums/StateMachineMessage.md) state)</div>|
|:---|
|发送一个当前状态机消息的通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">GetAnimationPostNotify</font> ()</div>|
|:---|
|获取动画完成通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">GetUpdateAssetNotify</font>](/Api/Classes/Animation/Animator_F/GetUpdateAssetNotify.md) ([constchar*](/Api/Enums/constchar*.md) url, [bool](/Api/DataType/Bool.md) state)</div>|
|:---|
|获取更新资源通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">UpdateAssetNotify</font>](/Api/Classes/Animation/Animator_F/UpdateAssetNotify.md) ([constchar*](/Api/Enums/constchar*.md) url, [bool](/Api/DataType/Bool.md) state)</div>|
|:---|
|更新资源通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">ClipsEventNotify</font>](/Api/Classes/Animation/Animator_F/ClipsEventNotify.md) ([constchar*](/Api/Enums/constchar*.md) function, [ReflexVariant](/Api/Enums/ReflexVariant.md) variant)</div>|
|:---|
|动画切片事件通知|

