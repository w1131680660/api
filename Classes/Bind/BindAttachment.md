# BindAttachment

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BoneName</font></div>|
|:---|
|绑点名字|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|绑点坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Euler</font></div>|
|:---|
|绑点欧拉角|

## 代码示例

```lua
--创建模型
local model = SandboxNode.new('Model', game.WorkSpace)
model.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100041")
model.Position = Vector3.new(500, 700, 150)
--给模型设置绑点
local attachment= SandboxNode.new('BindAttachment', model)
attachment.BoneName = 'attachment'
attachment.Position = Vector3.new(100, 0, 100)
attachment.Euler = Vector3.new(2, 1, 1)
```