# DefaultSound

## 属性

|<div style="width:700px">[EnumDefaultSound](/Api/Enums/EnumDefaultSound.md) &emsp;<font color="dd00dd">SoundType</font></div>|
|:---|
|默认声音类型枚举：脚步、行为、受击、待机、技能、环境、背景音乐、提示和其他|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EffectIndex</font></div>|
|:---|
|音效效果序列|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local Effect = SandboxNode.new('DefaultSound', part)
--设置音效为脚步
Effect.SoundType = Enum.Sound.FootStep
--设置音效序列
Effect.EffectIndex = 13
Effect:PlaySound() --播放音效
```