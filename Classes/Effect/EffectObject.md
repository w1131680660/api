# EffectObject

## 属性

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">AssetID</font></div>|
|:---|
|特效资源id|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Duration</font></div>|
|:---|
|特效持续时间|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Looping</font></div>|
|:---|
|特效是否循环|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">Material</font></div>|
|:---|
|轨迹材质路径|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Rate</font></div>|
|:---|
|特效进度|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TexturePath</font></div>|
|:---|
|纹理路径|

|<div style="width:700px">[EmitterTrailsMode](/Api/Enums/EmitterTrailsMode.md) &emsp;<font color="dd00dd">TrailsMode</font></div>|
|:---|
|轨迹模式|

|<div style="width:700px">[EmitterTrailsTextureMode](/Api/Enums/EmitterTrailsTextureMode.md) &emsp;<font color="dd00dd">TrailsTextureMode</font></div>|
|:---|
|轨迹纹理模式|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">SizeAffectsWidth</font></div>|
|:---|
|尺寸影响宽度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">InheritParticleColor</font></div>|
|:---|
|继承粒子颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ColorOverTrails</font></div>|
|:---|
|彩色覆盖轨迹|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TrailsTexturePath</font></div>|
|:---|
|轨迹纹理路径|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SimulationSpeed</font></div>|
|:---|
|播放速度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoDestory</font></div>|
|:---|
|自动销毁|

|<div style="width:700px">[EmitterColorOverLifeTimeMode](/Api/Enums/EmitterColorOverLifeTimeMode.md) &emsp;<font color="dd00dd">ColorOverLifeTimeMode</font></div>|
|:---|
|\t颜色随生命周期内变化模式|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ColorOverLifeTimeMinColor</font></div>|
|:---|
|\t颜色随生命周期内变化的最小颜色值|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ColorOverLifeTimeMaxColor</font></div>|
|:---|
|\t颜色随生命周期内变化的最大颜色值|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Prewarm</font></div>|
|:---|
|预热|

|<div style="width:700px">[ParticleSystemSimulationSpace](/Api/Enums/ParticleSystemSimulationSpace.md) &emsp;<font color="dd00dd">SimulationSpace</font></div>|
|:---|
|移动坐标系|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DeltaTime</font></div>|
|:---|
|单位时间|

|<div style="width:700px">[ParticleSystemScalingMode](/Api/Enums/ParticleSystemScalingMode.md) &emsp;<font color="dd00dd">ScalingMode</font></div>|
|:---|
|缩放模式|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">PlayOnAwake</font></div>|
|:---|
|创建时启动|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">MaxParticles</font></div>|
|:---|
|最大粒子数量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoRandomSeed</font></div>|
|:---|
|自动随机种子|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RandomSeed</font></div>|
|:---|
|随机种子|

|<div style="width:700px">[ParticleSystemCullingMode](/Api/Enums/ParticleSystemCullingMode.md) &emsp;<font color="dd00dd">CullingMode</font></div>|
|:---|
|裁剪模式|

|<div style="width:700px">[ParticleSystemRingBufferMode](/Api/Enums/ParticleSystemRingBufferMode.md) &emsp;<font color="dd00dd">RingBufferMode</font></div>|
|:---|
||

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">LoopRange</font></div>|
|:---|
|粒子循环生命区间|

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">StartColorGradient</font></div>|
|:---|
||

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TrailMaterial</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmissionBurst](/Api/Enums/ParticleEmissionBurst.md) &emsp;<font color="dd00dd">Brust</font></div>|
|:---|
|（爆发），产生粒子爆发的效果，通过Time（时间）、Count（数量）、Cycles（周期）、Interval（间隔）四个参数调整。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableSizeOverLifeTime</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">OverLifeTimeSize</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableRotationOverLifeTime</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableUV</font></div>|
|:---|
|开启uv模块|

|<div style="width:700px">[ParticleSystemUVMode](/Api/Enums/ParticleSystemUVMode.md) &emsp;<font color="dd00dd">UVMode</font></div>|
|:---|
|uv模式|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Tiles</font></div>|
|:---|
|Y（垂直）方向上划分的区块数量。|

|<div style="width:700px">[ParticleSystemUVGridType](/Api/Enums/ParticleSystemUVGridType.md) &emsp;<font color="dd00dd">Animation</font></div>|
|:---|
|动画模式|

|<div style="width:700px">[ParticleSystemUVRowMode](/Api/Enums/ParticleSystemUVRowMode.md) &emsp;<font color="dd00dd">RowMode</font></div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomRow</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemUVTimeMode](/Api/Enums/ParticleSystemUVTimeMode.md) &emsp;<font color="dd00dd">TimeMode</font></div>|
|:---|
||

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">SpeedRange</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FPS</font></div>|
|:---|
|根据指定的每秒帧数值对帧进行采样|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Cycles</font></div>|
|:---|
|动画序列在粒子生命周期内重复的次数。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableVelocityOverLifetime</font></div>|
|:---|
|是否开启|

|<div style="width:700px">[ParticleVelocityOverLifetimeSpaceMode](/Api/Enums/ParticleVelocityOverLifetimeSpaceMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpace</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableLimitVelocityOverLifetime</font></div>|
|:---|
|是否开启|

|<div style="width:700px">[ParticleLimitVelocityOverLifetimeSeparateAxes](/Api/Enums/ParticleLimitVelocityOverLifetimeSeparateAxes.md) &emsp;<font color="dd00dd">EnableSeparateAxes</font></div>|
|:---|
|分量。|

|<div style="width:700px">[ParticleLimitVelocityOverLifetimeSpaceMode](/Api/Enums/ParticleLimitVelocityOverLifetimeSpaceMode.md) &emsp;<font color="dd00dd">LimitVelocityOverLifeTimeSpace</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LimitVelocityOverLifeTimeDampen</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MultiplyBySize</font></div>|
|:---|
|启用此属性后，较大的粒子会更大程度上受到阻力系数的影响。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MultiplyByVelocity</font></div>|
|:---|
|启用此属性后，较快的粒子会更大程度上受到阻力系数的影响。|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TrailsRatio</font></div>|
|:---|
|随机分配轨迹，因此该值表示概率。|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TrailsMinVertexDistance</font></div>|
|:---|
|定义粒子在其轨迹接收新顶点之前必须经过的距离。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsWorldSpace</font></div>|
|:---|
|Space__，轨迹顶点也不会相对于粒子系统的游戏对象移动。相反，轨迹顶点将被置于世界空间中，并忽略粒子系统的任何移动|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsDieWithParticles</font></div>|
|:---|
|轨迹会在粒子死亡时立即消失|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TrailsRibbonCount</font></div>|
|:---|
|选择要在整个粒子系统中渲染的轨迹带数量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsSplitSubEmitterRibbons</font></div>|
|:---|
|在用作子发射器的系统上启用此属性时，从同一父系统粒子生成的粒子将共享一个轨迹带|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsAttachRibbonsToTransform</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsSizeAffectsLifetime</font></div>|
|:---|
|如果启用此属性（选中复选框），则轨迹生命周期受粒子大小影响。|

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">TrailsOverLifetimeColorMode</font></div>|
|:---|
|通过一条曲线控制整个轨迹在其附着粒子的整个生命周期内的颜色。|

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">TrailsOverMode</font></div>|
|:---|
|通过一条曲线控制轨迹沿其长度的颜色。|

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">TrailsOverGradient</font></div>|
|:---|
|通过一条曲线控制轨迹沿其长度的颜色。。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">TrailsGenerateLightingData</font></div>|
|:---|
|通过启用此属性（选中复选框），可在构建轨迹几何体时包含法线和切线。这样允许它们使用具有场景光照的材质，例如通过标准着色器，或通过使用自定义着色器。|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TrailsShadowBias</font></div>|
|:---|
||

|<div style="width:700px">[ParticleLineAlignment](/Api/Enums/ParticleLineAlignment.md) &emsp;<font color="dd00dd">TrailsAlignment</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableColorBySpeed</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">ColorBySpeedGradient</font></div>|
|:---|
|在速度范围内定义的粒子的颜色渐变。|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ColorBySpeedRange</font></div>|
|:---|
|颜色渐变映射到的速度范围的下限和上限（超出范围的速度将映射到渐变的端点）。。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableSizeBySpeed</font></div>|
|:---|
||

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">SizeBySpeedRange</font></div>|
|:---|
|大小曲线映射到的速度范围的下限和上限（超出范围的速度将映射到曲线的端点）。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableRotationBySpeed</font></div>|
|:---|
||

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">RotationBySpeedRange</font></div>|
|:---|
|大小曲线映射到的速度范围的下限和上限（超出范围的速度将映射到曲线的端点）。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableNoise</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseFrequency</font></div>|
|:---|
|此属性可控制粒子改变行进方向的频率以及方向变化的突然程度。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">NoiseDamping</font></div>|
|:---|
|启用此属性后，强度与频率成正比。|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseOctaveCount</font></div>|
|:---|
|指定组合多少层重叠噪声来产生最终噪声值。|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseOctaveMultiplier</font></div>|
|:---|
|对于每个附加的噪声层，按此比例降低强度。|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseOctaveScale</font></div>|
|:---|
|对于每个附加的噪声层，按此乘数调整频率。|

|<div style="width:700px">[ParticleQualityDropdown](/Api/Enums/ParticleQualityDropdown.md) &emsp;<font color="dd00dd">NoiseQuality</font></div>|
|:---|
|较低的质量设置可显著降低性能成本，但也会影响噪声的有趣程度。请使用能为您提供所需行为的最低质量以获得最佳性能。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">NoiseRemapEnabled</font></div>|
|:---|
|将最终噪声值重新映射到不同的范围。|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableCustomData</font></div>|
|:---|
||

|<div style="width:700px">[ParticleCustomDataMode](/Api/Enums/ParticleCustomDataMode.md) &emsp;<font color="dd00dd">CustomDataMode1</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">CustomDataColorMode1</font></div>|
|:---|
||

|<div style="width:700px">[ParticleCustomDataMode](/Api/Enums/ParticleCustomDataMode.md) &emsp;<font color="dd00dd">CustomDataMode2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">CustomDataColorMode2</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableShape</font></div>|
|:---|
||

|<div style="width:700px">[EmitterShape](/Api/Enums/EmitterShape.md) &emsp;<font color="dd00dd">ShapeType</font></div>|
|:---|
|特效类型|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeRadius</font></div>|
|:---|
|形状的圆形半径|

|<div style="width:700px">[ParticleShapeMeshSpawnMode](/Api/Enums/ParticleShapeMeshSpawnMode.md) &emsp;<font color="dd00dd">ShapeRadiusMode</font></div>|
|:---|
|如何在形状的弧形周围生成粒子|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeRadiusSpread</font></div>|
|:---|
|弧形周围可产生粒子的离散间隔|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeRadiusThickness</font></div>|
|:---|
|发射粒子的体积比例|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeArc</font></div>|
|:---|
|形成发射器形状的整圆的角部。|

|<div style="width:700px">[ParticleShapeMeshSpawnMode](/Api/Enums/ParticleShapeMeshSpawnMode.md) &emsp;<font color="dd00dd">ShapeArcMode</font></div>|
|:---|
|如何在形状的弧形周围生成粒子|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeArcSpread</font></div>|
|:---|
|弧形周围可产生粒子的离散间隔|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeAngle</font></div>|
|:---|
|锥体在其顶点处的角度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeLength</font></div>|
|:---|
|锥体的长度|

|<div style="width:700px">[ParticleShapeConeType](/Api/Enums/ParticleShapeConeType.md) &emsp;<font color="dd00dd">ShapeConeType</font></div>|
|:---|
|Cone类型|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeDonutRadius</font></div>|
|:---|
|外圆环的粗度|

|<div style="width:700px">[ParticleShapeBoxType](/Api/Enums/ParticleShapeBoxType.md) &emsp;<font color="dd00dd">ShapeBoxType</font></div>|
|:---|
|Box类型|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">ShapeBoxThickness</font></div>|
|:---|
|发射粒子的体积比例|

|<div style="width:700px">[ParticleShapeMeshType](/Api/Enums/ParticleShapeMeshType.md) &emsp;<font color="dd00dd">ShapeMeshType</font></div>|
|:---|
|mesh类型|

|<div style="width:700px">[ParticleShapeMeshSpawnMode](/Api/Enums/ParticleShapeMeshSpawnMode.md) &emsp;<font color="dd00dd">ShapeMeshSpawnMode</font></div>|
|:---|
|如何在形状的弧形周围生成粒子|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpread</font></div>|
|:---|
|弧形周围可产生粒子的离散间隔|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">StartLifetimeState</font></div>|
|:---|
|特效生命周期|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">StartSpeedState</font></div>|
|:---|
|开始速度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">GravityModifierState</font></div>|
|:---|
|重力|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">RateOverTimeState</font></div>|
|:---|
|（随时间的速率），每单位时间发射的粒子数量|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">RateOverDistanceState</font></div>|
|:---|
|（通过距离的速率），每单位距离发射的粒子数量|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">FrameOverTimeState</font></div>|
|:---|
|通过一条曲线指定动画帧随着时间的推移如何增加|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearState</font></div>|
|:---|
|X，Y和Z轴的速度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalState</font></div>|
|:---|
|轴的轨道速度。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetState</font></div>|
|:---|
|轨道中心的位置，适用于轨道运行粒子。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeRadialState</font></div>|
|:---|
|粒子远离/朝向中心位置的径向速度。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpeedModifierState</font></div>|
|:---|
|在当前行进方向上/周围向粒子的速度应用一个乘数。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">TrailsLifetimeState</font></div>|
|:---|
|轨迹中每个顶点的生命周期，表示为所属粒子的生命周期的乘数。当每个新顶点添加到轨迹时，该顶点将在其存在时间超过其总生命周期后消失。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">WidthOverTrailsState</font></div>|
|:---|
|轨迹上方的宽度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoiseScrollSpeedState</font></div>|
|:---|
|随着时间的推移而移动噪声场可产生更不可预测和不稳定的粒子移动|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoiseRemapState</font></div>|
|:---|
|将最终噪声值重新映射到不同的范围|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoisePositionAmountState</font></div>|
|:---|
|用于控制噪声对粒子位置影响程度的乘数|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoiseRotationAmountState</font></div>|
|:---|
|用于控制噪声对粒子旋转（以度/秒为单位）影响程度的乘数。|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoiseSizeAmountState</font></div>|
|:---|
|用于控制噪声对粒子大小影响程度的乘数|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">ShapeRadiusSpeedState</font></div>|
|:---|
|发射位置围绕弧形移动的速度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">ShapeArcSpeedState</font></div>|
|:---|
|发射位置围绕弧形移动的速度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpeedState</font></div>|
|:---|
|发射位置围绕弧形移动的速度|

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorX1State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorY1State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorZ1State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorW1State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorX2State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorY2State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorZ2State</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">CustomDataVectorW2State</font></div>|
|:---|
||

|<div style="width:700px">[CullLayer](/Api/Enums/CullLayer.md) &emsp;<font color="dd00dd">CullLayer</font></div>|
|:---|
|消隐层|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IgnoreStreamSync</font></div>|
|:---|
|忽略流同步|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ChildAutoPlay</font></div>|
|:---|
|子节点是否自动播放|

|<div style="width:700px">[EnumParticleSystemOnlyConstantCurveMode](/Api/Enums/EnumParticleSystemOnlyConstantCurveMode.md) &emsp;<font color="dd00dd">StartDelayState</font></div>|
|:---|
|开始延迟配置|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartDelayConstant</font></div>|
|:---|
|开始延迟单常量|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">StartDelayTwoConstant</font></div>|
|:---|
|开始延迟双常量|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartLifeTimeConstant</font></div>|
|:---|
|开始生命周期单常量|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">StartLifeTimeTwoConstant</font></div>|
|:---|
|开始生命周期双常量|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">StartLifeTimeCurve</font></div>|
|:---|
|开始生命周期双常量|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">StartLifeTimeTwoCurve</font></div>|
|:---|
|开始生命周期双常量|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartSpeedConstant</font></div>|
|:---|
|开始速度单常量|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">StartSpeedTwoConstant</font></div>|
|:---|
|开始速度双常量|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">StartSpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">StartSpeedTwoCurve</font></div>|
|:---|
|开始速度双曲线|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Start3DSizeSeparate</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">Start3DSizeState</font></div>|
|:---|
|特效尺寸|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DSizeXConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DSizeXTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeXCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeXTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DSizeYConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DSizeYTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeYCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeYTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DSizeZConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DSizeZTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeZCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DSizeZTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Start3DRotationSeparate</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">Start3DRotationState</font></div>|
|:---|
|特效尺寸|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DRotationZConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DRotationZTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationZCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationZTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DRotationYConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DRotationYTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationYCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationYTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Start3DRotationXConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">Start3DRotationXTwoConstant</font></div>|
|:---|
|[|

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationXCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">Start3DRotationXTwoCurve</font></div>|
|:---|
|[|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FlipRotation</font></div>|
|:---|
|[|

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">StartColorState</font></div>|
|:---|
|粒子颜色方式|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">StartColorQuad</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">StartColorQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">StartColorGradient2</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GravityModifierConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">GravityModifierTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">GravityModifierOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">GravityModifierTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RateOverTimeConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">RateOverTimeTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RateOverTimeOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RateOverTimeTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RateOverDistanceConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">RateOverDistanceTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RateOverDistanceOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RateOverDistanceTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeRadiusSpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">ShapeRadiusSpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">ShapeRadiusSpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">ShapeRadiusSpeedTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeArcSpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">ShapeArcSpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">ShapeArcSpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">ShapeArcSpeedTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">ShapeMeshSpawnSpeedTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeLinearZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOrbitalZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeOffsetZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeRadialConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeRadialTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeRadialOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeRadialTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpeedModifierConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpeedModifierTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpeedModifierOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">VelocityOverLifeTimeSpeedModifierTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">LimitVelocitySpeedState</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LimitVelocitySpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">LimitVelocitySpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySpeedTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">LimitVelocitySeparateSpeedZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">LimitVelocityDragState</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LimitVelocityDragConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">LimitVelocityDragTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">LimitVelocityDragOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">LimitVelocityDragTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemGradientMode](/Api/Enums/ParticleSystemGradientMode.md) &emsp;<font color="dd00dd">ColorBySpeedState</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ColorBySpeedQuad</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">ColorBySpeedQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">ColorBySpeedGradient2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">SizeOverLifeState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">SizeOverLifeConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">SizeOverLifeTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeOverLifeZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableSizeOverLifeSeparateAxes</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">SizeBySpeedState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">SizeBySpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">SizeBySpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">SizeBySpeedZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">RotationOverLifeState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">RotationOverLifeConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">RotationOverLifeTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationOverLifeZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">RotationBySpeedState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">RotationBySpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">RotationBySpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">RotationBySpeedZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ParticleSystemCurveMode](/Api/Enums/ParticleSystemCurveMode.md) &emsp;<font color="dd00dd">NoiseStrengthState</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">NoiseStrengthConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">NoiseStrengthTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseStrengthZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseScrollSpeedConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">NoiseScrollSpeedTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseScrollSpeedOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseScrollSpeedTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">NoiseRemapConstant</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">NoiseRemapTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapXOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapXTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapYOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapYTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseRemapZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoisePositionAmountConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">NoisePositionAmountTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoisePositionAmountOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoisePositionAmountTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseRotationAmountConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">NoiseRotationAmountTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseRotationAmountOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseRotationAmountTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">NoiseSizeAmountConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">NoiseSizeAmountTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">NoiseSizeAmountOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">NoiseSizeAmountTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FrameOverTimeConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">FrameOverTimeTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">FrameOverTimeOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">FrameOverTimeTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[EnumParticleSystemOnlyConstantCurveMode](/Api/Enums/EnumParticleSystemOnlyConstantCurveMode.md) &emsp;<font color="dd00dd">UVStartFrameState</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">UVStartFrameConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">UVStartFrameTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TrailsLifetimeConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">TrailsLifetimeTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">TrailsLifetimeOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">TrailsLifetimeTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TrailsOverLifetimeColorQuad</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">TrailsOverLifetimeColorGradient</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TrailsOverLifetimeQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">TrailsOverLifetimeGradient2</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">WidthOverTrailsConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">WidthOverTrailsTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">WidthOverTrailsOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">WidthOverTrailsTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TrailsOverQuad</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">TrailsOverGradient</font></div>|
|:---|
|通过一条曲线控制轨迹沿其长度的颜色。。|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TrailsOverQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">TrailsOverGradient2</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">CustomData1ColorQuad</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">CustomData1ColorGradient</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">CustomData1ColorQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">CustomData1ColorGradient2</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData1XConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData1XTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData1XOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData1XTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData1YConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData1YTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData1YOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData1YTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData1ZConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData1ZTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData1ZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData1ZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData1WConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData1WTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData1WOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData1WTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">CustomData2ColorQuad</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">CustomData2ColorGradient</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">CustomData2ColorQuad2</font></div>|
|:---|
||

|<div style="width:700px">[ParticleEmitterColorGradient](/Api/Enums/ParticleEmitterColorGradient.md) &emsp;<font color="dd00dd">CustomData2ColorGradient2</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData2XConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData2XTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData2XOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData2XTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData2YConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData2YTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData2YOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData2YTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData2ZConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData2ZTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData2ZOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData2ZTwoCurve</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CustomData2WConstant</font></div>|
|:---|
||

|<div style="width:700px">[RangeInfo](/Api/DataType/RangeInfo.md) &emsp;<font color="dd00dd">CustomData2WTwoConstant</font></div>|
|:---|
||

|<div style="width:700px">[FloatCurve](/Api/Enums/FloatCurve.md) &emsp;<font color="dd00dd">CustomData2WOneCurve</font></div>|
|:---|
||

|<div style="width:700px">[RangeFloatCurve](/Api/Enums/RangeFloatCurve.md) &emsp;<font color="dd00dd">CustomData2WTwoCurve</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Test</font> ()</div>|
|:---|
|测试|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAssetID</font>](/Api/Classes/Effect/EffectObject_F/SetAssetID.md) ([ModelAssetType](/Api/DataType/ModelAssetType.md) assetID, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置资源id|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Start</font> ()</div>|
|:---|
|特效开始播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Pause</font> ()</div>|
|:---|
|特效暂停播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ReStart</font> ()</div>|
|:---|
|特效重新开始播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Stop</font>](/Api/Classes/Effect/EffectObject_F/Stop.md) ([int](/Api/DataType/Number.md) behavior)</div>|
|:---|
|特效停止播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMinGradientColors</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMinGradientColors.md) ([int](/Api/DataType/Number.md) idx, [float](/Api/DataType/Number.md) time, [ColorQuad](/Api/DataType/ColorQuad.md) color)</div>|
|:---|
|修改ColorOverLifeTime的minGradient的_colors|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMaxGradientColors</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMaxGradientColors.md) ([int](/Api/DataType/Number.md) idx, [float](/Api/DataType/Number.md) time, [ColorQuad](/Api/DataType/ColorQuad.md) color)</div>|
|:---|
|修改ColorOverLifeTime的maxGradient的_colors|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMinGradientAlphas</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMinGradientAlphas.md) ([int](/Api/DataType/Number.md) idx, [float](/Api/DataType/Number.md) time, [int](/Api/DataType/Number.md) alpha)</div>|
|:---|
|修改ColorOverLifeTime的minGradient的_alphas|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMaxGradientAlphas</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMaxGradientAlphas.md) ([int](/Api/DataType/Number.md) idx, [float](/Api/DataType/Number.md) time, [int](/Api/DataType/Number.md) alpha)</div>|
|:---|
|修改ColorOverLifeTime的maxGradient的_alphas|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMinGradientModeAndKey</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMinGradientModeAndKey.md) ([int](/Api/DataType/Number.md) mode, [int](/Api/DataType/Number.md) colorkey, [int](/Api/DataType/Number.md) alphakey)</div>|
|:---|
|修改ColorOverLifeTime的minGradient的mode|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetCOLTMaxGradientModeAndKey</font>](/Api/Classes/Effect/EffectObject_F/SetCOLTMaxGradientModeAndKey.md) ([int](/Api/DataType/Number.md) mode, [int](/Api/DataType/Number.md) colorkey, [int](/Api/DataType/Number.md) alphakey)</div>|
|:---|
|修改ColorOverLifeTime的maxGradient的mode|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">StopPlaying</font>](/Api/Classes/Effect/EffectObject_F/StopPlaying.md) ([bool](/Api/DataType/Bool.md) isStop)</div>|
|:---|
|停止播放时触发|

