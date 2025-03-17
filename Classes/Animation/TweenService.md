# TweenService

## 成员函数

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">Create</font>](/Api/Classes/Animation/TweenService_F/Create.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [TweenInfo](/Api/DataType/TweenInfo.md) info, [ReflexMap](/Api/Enums/ReflexMap.md) map)</div>|
|:---|
|将暂停补间动画的播放|

## 代码示例

```lua
--创建实例
--创建实例
local TweenService = game:GetService('TweenService')
--缓动数据
local TweenInfo = TweenInfo.new(3.0, Enum.EasingStyle.Linear, nil, 0, 1)
--创建一个button
local root = SandboxNode.new('UIRoot', game.WorkSpace)
root.Name = 'uiroot'
local button= SandboxNode.new('UIButton', game.WorkSpace.uiroot)
button.Icon = 'ui\\mobile\\texture0\\common\\board_activity_box_white.png'
button.Size = Vector2.new(100, 50)
button.Position = Vector2.new(200, 100)
local goal = {}
goal.Position = Vector2.new(300, 200)
--创建缓动
local tween = TweenService:Create(button, TweenInfo, goal)
--缓动播放
tween:Play()
--缓动停止
tween:Pause()
--缓动继续
tween:Resume()
--缓动取消
tween:Cancel()
```