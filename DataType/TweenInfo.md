# TweenInfo
------------------------------------------------------------------------------------------
## 描述

包括如何使用 TweenInfo 数据类型对 Tween 进行插值的信息。TweenInfo 数据类型包括一系列属性，可用于实现各种风格的动画效果，包括反转和循环

------------------------------------------------------------------------------------------
## 属性

|<div style="width:700px">[TweenInfo](/Api/DataType/TweenInfo.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
|:---|
|构造|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">EasingDirection</font>]()</div>|
|:---|
|缓动方向|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Time</font>]()</div>|
|:---|
|缓动时间|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">DelayTime</font>]()</div>|
|:---|
|延迟时间|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">RepeatCount</font>]()</div>|
|:---|
|循环次数。小于零时 tween 会无限循环|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">EasingStyle</font>]()</div>|
|:---|
|释放样式|

|<div style="width:700px">[Bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Reverses</font>]()</div>|
|:---|
|tween 完成目标后会否反转|


------------------------------------------------------------------------------------------
## 示例代码

```lua
--缓动数据
-- 所有参数为默认的 TweenInfo
local default = TweenInfo.New() 
 
-- 时间设置为 0.5 秒的 TweenInfo
local timeChanged = TweenInfo.New(0.5) 
 
-- 释放样式设置为 Back 的 TweenInfo
local easingStyled = TweenInfo.New(0.5, Enum.EasingStyle.Back, 0, 0, 0, false) 
 
-- 释放方向设置为 In 的 TweenInfo
local easingDirected = TweenInfo.New(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.In, 0, 0, false)
 
-- 自身重复 4 次的 TweenInfo
local repeated = TweenInfo.New(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.In, 0, 4, false)
 
-- 完成目标后会反向其插值的 TweenInfo
local reverses = TweenInfo.New(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.In, 0, 4, true)
 
-- 无限循环的 TweenInfo
local reverses = TweenInfo.New(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.In, 0, -1,  true)
 
-- 各插值之间有 1 秒延迟的 TweenInfo
local delayed = TweenInfo.New(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.In, 1, 4, true)
```

循环Tween
```lua
local TweenService = game:GetService("TweenService")
 
local part = Sandbox.New("Part")
part.Position = Vector3.New(0, 10, 0)
part.Anchored = true
part.Parent = game.Workspace
 
local tweenInfo = TweenInfo.New(
    2, -- Time
    Enum.EasingStyle.Linear, -- EasingStyle
	Enum.EasingDirection.Out, -- EasingDirection
	0 -- DelayTime
	-1, -- RepeatCount (小于零时 tween 会无限循环)
	true, -- Reverses (tween 完成目标后会反转)
)
 
local tween = TweenService:Create(part, tweenInfo, {Position = Vector3.New(0, 30, 0)})
 
tween:Play()
wait(10)
tween:Cancel() -- 在 10 秒后取消动画
```