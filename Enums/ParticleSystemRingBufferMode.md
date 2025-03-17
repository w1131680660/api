# ParticleSystemRingBufferMode

------------------------------------------------------------------------------------------
## 描述

发射器粒子循环利用方式：控制如何从粒子系统中移除粒子

------------------------------------------------------------------------------------------
## 枚举

|<div style="width:200px">ParticleSystemRingBufferMode</div>|<div style="width:100px"></div>|<div style="width:100px"></div>|
|:---|:---|:---|
|**名称**|**值**|**描述**|
|Disabled|1|当粒子的存活时间超过它们的生命周期时，将移除粒子|
|PauseUntilReplaced|2|创建新粒子会超过MaxParticles属性时将移除粒子|
|LoopUntilReplaced|3|创建新粒子会超过MaxParticles属性时将移除粒子。在移除粒子之前，粒子保持存活，直到它们的存活时间超过它们的生命周期|
