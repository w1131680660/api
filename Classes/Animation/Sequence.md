# Sequence

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">SequenceId</font></div>|
|:---|
|动画序列ID|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Time</font></div>|
|:---|
|动画时长|

## 代码示例

```lua
--local animation
--创建SandboxSequenceObject
local sequenceNode = SandboxNode.new('Sequence')
sequenceNode:SetParent(game.WorkSpace)--animation
sequenceNode.SequenceId = 'id1'
sequenceNode.Time= 10
```