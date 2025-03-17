# DefaultEffect

## 属性

|<div style="width:700px">[EnumDefaultEffect](/Api/Enums/EnumDefaultEffect.md) &emsp;<font color="dd00dd">EffectType</font></div>|
|:---|
|特效效果类型,有烟雾、爆炸、光效、粒子、火焰、环境和提示|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EffectIndex</font></div>|
|:---|
|特效效果序列|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Scale</font></div>|
|:---|
|整体缩放比例|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Visible</font></div>|
|:---|
|是否显示视觉效果|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">MaxTime</font></div>|
|:---|
|特效持续时长|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">VisibleDistance</font></div>|
|:---|
|特效最大可见距离|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">AssetID</font></div>|
|:---|
|资源ID|

|<div style="width:700px">[CullLayer](/Api/Enums/CullLayer.md) &emsp;<font color="dd00dd">CullLayer</font></div>|
|:---|
|消隐层|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local Effect = SandboxNode.new('DefaultEffect', workspace)
local pos2 = Vector3.new(unpack({1000,1000,1000}))
--设置特效位置
Effect.Position = pos2
--设置特效为火焰类型
Effect.EffectType = Enum.Effect.Fire
--设置特效序列
Effect.EffectIndex = 13
--设置特效时长
Effect.MaxTime = 10
--设置特效可见距离
Effect.VisibleDistance = 100
```