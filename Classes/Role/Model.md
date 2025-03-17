# Model

## 属性

|<div style="width:700px">[DimensionUnit](/Api/Enums/DimensionUnit.md) &emsp;<font color="dd00dd">DimensionUnit</font></div>|
|:---|
|模型尺寸|

|<div style="width:700px">[MaterialTemplate](/Api/Enums/MaterialTemplate.md) &emsp;<font color="dd00dd">MaterialType</font></div>|
|:---|
|材料类型|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TextureId</font></div>|
|:---|
|设置模型的材质，即资源id|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">Color</font></div>|
|:---|
|模型的颜色|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">ModelId</font></div>|
|:---|
|模型id，即资源id|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Gravity</font></div>|
|:---|
|模型重力|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Friction</font></div>|
|:---|
|模型摩擦力|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Restitution</font></div>|
|:---|
|模型反弹力，比如物体撞击在地面上会根据此值来计算反弹高度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Mass</font></div>|
|:---|
|模型质量|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Velocity</font></div>|
|:---|
|模型移动速度|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">AngleVelocity</font></div>|
|:---|
|模型角速度|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Size</font></div>|
|:---|
|模型的包围盒大小|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Center</font></div>|
|:---|
|模型的中心点所在世界坐标|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableGravity</font></div>|
|:---|
|模型是否支持重力|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Anchored</font></div>|
|:---|
|锚定状态，为true时此物体不受外部环境物理影响，但是会给外部提供物理输入。例如：有外来物体撞击到此物体，此物体不会产生移动，但是会对外来物体产生碰撞反弹力。|

|<div style="width:700px">[PhysicsType](/Api/Enums/PhysicsType.md) &emsp;<font color="dd00dd">PhysXType</font></div>|
|:---|
|物理类型|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnablePhysics</font></div>|
|:---|
|开启此物体的物理状态。为true时物体的物理属性可以使用|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanCollide</font></div>|
|:---|
|是否可以碰撞。设为false时为trigger状态|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanTouch</font></div>|
|:---|
|是否触发碰撞回调函数：Touched和TouchEnded事件|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CollideGroupID</font></div>|
|:---|
|int)，可以通过PhysXService:SetCollideInfo函数设置任意两个组之间是否会产生碰撞|

|<div style="width:700px">[CullLayer](/Api/Enums/CullLayer.md) &emsp;<font color="dd00dd">CullLayer</font></div>|
|:---|
|消隐层|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IgnoreStreamSync</font></div>|
|:---|
|忽略流同步|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TextureOverride</font></div>|
|:---|
|材质贴图覆盖|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CastShadow</font></div>|
|:---|
|是否打开阴影|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanRideOn</font></div>|
|:---|
|能否跟着走|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DrawPhysicsCollider</font></div>|
|:---|
|显示物理包围盒|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ReceiveShadow</font></div>|
|:---|
|是否接受投影|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanBePushed</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsStatic</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">OutlineActive</font></div>|
|:---|
|是否激活描边|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">OutlineColorIndex</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">PlayAnimation</font>](/Api/Classes/Role/Model_F/PlayAnimation.md) ([string](/Api/DataType/String.md) id, [float](/Api/DataType/Number.md) speed, [int](/Api/DataType/Number.md) loop)</div>|
|:---|
|播放动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">PlayAnimationEx</font>](/Api/Classes/Role/Model_F/PlayAnimationEx.md) ([string](/Api/DataType/String.md) id, [float](/Api/DataType/Number.md) speed, [int](/Api/DataType/Number.md) loop, [int](/Api/DataType/Number.md) priority, [float](/Api/DataType/Number.md) weight)</div>|
|:---|
|播放动画Ex|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">StopAnimation</font>](/Api/Classes/Role/Model_F/StopAnimation.md) ([string](/Api/DataType/String.md) id)</div>|
|:---|
|停止动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">StopAnimationEx</font>](/Api/Classes/Role/Model_F/StopAnimationEx.md) ([string](/Api/DataType/String.md) id, [bool](/Api/DataType/Bool.md) reset)</div>|
|:---|
|停止动画Ex|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">StopAllAnimation</font>](/Api/Classes/Role/Model_F/StopAllAnimation.md) ([bool](/Api/DataType/Bool.md) reset)</div>|
|:---|
|停止所有动画|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">EnableAnimationEvent</font>](/Api/Classes/Role/Model_F/EnableAnimationEvent.md) ([bool](/Api/DataType/Bool.md) enable)</div>|
|:---|
|开启或关闭动画事件|

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;[<font color="dd00dd">GetAnimationIDs</font>](/Api/Classes/Role/Model_F/GetAnimationIDs.md) ()</div>|
|:---|
|获取动画ID|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetAnimationPriority</font>](/Api/Classes/Role/Model_F/GetAnimationPriority.md) ([int](/Api/DataType/Number.md) seqid)</div>|
|:---|
|获取动画优先级|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAnimationPriority</font>](/Api/Classes/Role/Model_F/SetAnimationPriority.md) ([int](/Api/DataType/Number.md) seqid, [int](/Api/DataType/Number.md) value)</div>|
|:---|
|设置动画优先级|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetAnimationWeight</font>](/Api/Classes/Role/Model_F/GetAnimationWeight.md) ([int](/Api/DataType/Number.md) seqid)</div>|
|:---|
|获取动画权重|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAnimationWeight</font>](/Api/Classes/Role/Model_F/SetAnimationWeight.md) ([int](/Api/DataType/Number.md) seqid, [float](/Api/DataType/Number.md) value)</div>|
|:---|
|设置动画权重|

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;[<font color="dd00dd">GetBones</font>](/Api/Classes/Role/Model_F/GetBones.md) ()</div>|
|:---|
|获取动画骨骼|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetBoneRotate</font>](/Api/Classes/Role/Model_F/SetBoneRotate.md) ([string](/Api/DataType/String.md) boneName, [Quaternion](/Api/DataType/Quaternion.md) qua, [float](/Api/DataType/Number.md) scale)</div>|
|:---|
|设置骨骼动画旋转|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">AnchorWorldPos</font>](/Api/Classes/Role/Model_F/AnchorWorldPos.md) ([int](/Api/DataType/Number.md) id, [Vector3](/Api/DataType/Vector3.md) offset)</div>|
|:---|
|获取锚点世界坐标（仅脚本可用）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsBinded</font>](/Api/Classes/Role/Model_F/IsBinded.md) ([bool](/Api/DataType/Bool.md) set)</div>|
|:---|
|是否绑定|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AddForce</font>](/Api/Classes/Role/Model_F/AddForce.md) ([Vector3](/Api/DataType/Vector3.md) force)</div>|
|:---|
|添加力|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AddTorque</font>](/Api/Classes/Role/Model_F/AddTorque.md) ([Vector3](/Api/DataType/Vector3.md) torque)</div>|
|:---|
|添加扭矩|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AddForceAtPosition</font>](/Api/Classes/Role/Model_F/AddForceAtPosition.md) ([Vector3](/Api/DataType/Vector3.md) force, [Vector3](/Api/DataType/Vector3.md) position, [int](/Api/DataType/Number.md) mode)</div>|
|:---|
|添加力位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMaterial</font>](/Api/Classes/Role/Model_F/SetMaterial.md) ([string](/Api/DataType/String.md) skinMeshRenderCompName, [string](/Api/DataType/String.md) materialid, [int](/Api/DataType/Number.md) index)</div>|
|:---|
|设置材质|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">SetMaterialNew</font>](/Api/Classes/Role/Model_F/SetMaterialNew.md) ([string](/Api/DataType/String.md) meshRenderCompName, [string](/Api/DataType/String.md) materialid, [int](/Api/DataType/Number.md) index, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置材质|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetMaterialByNameOrIndex</font>](/Api/Classes/Role/Model_F/GetMaterialByNameOrIndex.md) ([string](/Api/DataType/String.md) findKey, [bool](/Api/DataType/Bool.md) byName, [bool](/Api/DataType/Bool.md) isSkinMeshRender, [int](/Api/DataType/Number.md) materialIndex)</div>|
|:---|
|获取材质节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMaterialByNameOrIndex</font>](/Api/Classes/Role/Model_F/SetMaterialByNameOrIndex.md) ([string](/Api/DataType/String.md) findKey, [bool](/Api/DataType/Bool.md) byName, [bool](/Api/DataType/Bool.md) isSkinMeshRender, [int](/Api/DataType/Number.md) materialIndex, [string](/Api/DataType/String.md) resId, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置材质|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetLegacyAnimation</font>](/Api/Classes/Role/Model_F/GetLegacyAnimation.md) ()</div>|
|:---|
|获取骨骼动画|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetAnimation</font>](/Api/Classes/Role/Model_F/GetAnimation.md) ()</div>|
|:---|
|获取模型动画|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetAttributeAnimation</font>](/Api/Classes/Role/Model_F/GetAttributeAnimation.md) ()</div>|
|:---|
|获取属性动画|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSkeletonAnimation</font>](/Api/Classes/Role/Model_F/GetSkeletonAnimation.md) ()</div>|
|:---|
|获取骨骼动画|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetHumanAnimation</font>](/Api/Classes/Role/Model_F/GetHumanAnimation.md) ()</div>|
|:---|
|获取人形动画|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetAnimator</font>](/Api/Classes/Role/Model_F/GetAnimator.md) ()</div>|
|:---|
|获取动画制作器|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetMaterialInstance</font>](/Api/Classes/Role/Model_F/GetMaterialInstance.md) ([table](/Api/DataType/Table.md) ids, [uint32_t](/Api/Enums/uint32_t.md) idx)</div>|
|:---|
|获取材料实例|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsLoadFinish</font>](/Api/Classes/Role/Model_F/IsLoadFinish.md) ()</div>|
|:---|
|是否加载完成|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">GetRenderPosition</font>](/Api/Classes/Role/Model_F/GetRenderPosition.md) ()</div>|
|:---|
|获取渲染位置|

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;[<font color="dd00dd">GetRenderRotation</font>](/Api/Classes/Role/Model_F/GetRenderRotation.md) ()</div>|
|:---|
|获取渲染旋转|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">GetRenderEuler</font>](/Api/Classes/Role/Model_F/GetRenderEuler.md) ()</div>|
|:---|
|获取渲染欧拉角|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetBoneNodeChildByName</font>](/Api/Classes/Role/Model_F/GetBoneNodeChildByName.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) parentBoneNode, [string](/Api/DataType/String.md) name)</div>|
|:---|
|通过节点名查询该骨骼节点对象|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetBoneNodeByName</font>](/Api/Classes/Role/Model_F/GetBoneNodeByName.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|按名称获取骨骼节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMaterialResId</font>](/Api/Classes/Role/Model_F/SetMaterialResId.md) ([string](/Api/DataType/String.md) materialResId)</div>|
|:---|
|设置材质资源实例|

|<div style="width:700px">[0,1,2](/Api/Enums/0,1,2.md) &emsp;[<font color="dd00dd">GetLoadedResType</font>](/Api/Classes/Role/Model_F/GetLoadedResType.md) ()</div>|
|:---|
|获取已经加载的资源类型|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetAssetContent</font>](/Api/Classes/Role/Model_F/GetAssetContent.md) ([table](/Api/DataType/Table.md) , [AssetResType](/Api/Enums/AssetResType.md) , [int](/Api/DataType/Number.md) )</div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetAssetContent</font>](/Api/Classes/Role/Model_F/SetAssetContent.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) , [table](/Api/DataType/Table.md) , [int](/Api/DataType/Number.md) )</div>|
|:---|
||

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSnapShot</font>](/Api/Classes/Role/Model_F/GetSnapShot.md) ()</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetRenderersShadow</font>](/Api/Classes/Role/Model_F/SetRenderersShadow.md) ([string](/Api/DataType/String.md) , [int](/Api/DataType/Number.md) , [bool](/Api/DataType/Bool.md) )</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetRendererShadow</font>](/Api/Classes/Role/Model_F/SetRendererShadow.md) ([table](/Api/DataType/Table.md) , [int](/Api/DataType/Number.md) , [bool](/Api/DataType/Bool.md) )</div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Touched</font>](/Api/Classes/Role/Model_F/Touched.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [Vector3](/Api/DataType/Vector3.md) pos, [Vector3](/Api/DataType/Vector3.md) normal)</div>|
|:---|
|模型被其他模型碰撞时，会触发一个Touched通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TouchEnded</font>](/Api/Classes/Role/Model_F/TouchEnded.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|模型被其他模型碰撞结束时，会触发一个TouchEnded通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">AnimationEvent</font>](/Api/Classes/Role/Model_F/AnimationEvent.md) ([int](/Api/DataType/Number.md) a, [int](/Api/DataType/Number.md) b)</div>|
|:---|
|模型触发动画事件时发送一个AnimationEvent通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">AnimationFrameEvent</font>](/Api/Classes/Role/Model_F/AnimationFrameEvent.md) ([int](/Api/DataType/Number.md) a, [constchar*](/Api/Enums/constchar*.md) b, [int](/Api/DataType/Number.md) c)</div>|
|:---|
|动画帧事件触发|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">LoadFinish</font>](/Api/Classes/Role/Model_F/LoadFinish.md) ([bool](/Api/DataType/Bool.md) isFinish)</div>|
|:---|
|加载完成时触发事件|

## 代码示例

```lua
--创建实例
local newModel= SandboxNode.new('Model')
--设置名字
newModel.Name = "my_model"
--设置模型
newModel.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100010")
--设置位置
newModel.Position = Vector3.new(500,700,500)
--设置父节点 将模型节点添加到Workspace中
newModel:SetParent(Workspace)

--播放动画
local player = game:GetService("Players").LocalPlayer.Character
player:PlayAnimation("100114", 1.0, 0, 1, 1.0) --"100114 吃的动作"
player:StopAnimation("100114") --"100114 某个指定动作"
```