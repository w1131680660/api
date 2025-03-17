# UIVideoImage

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">FileName</font></div>|
|:---|
|视频影像资源路径|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Loop</font></div>|
|:---|
|循环播放|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Play</font></div>|
|:---|
|播放|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local root = SandboxNode.new('UIRoot',workspace)
local npcOneVideo = SandboxNode.new('UIVideoImage', root)
--设置节点名字
npcOneVideo.Name = "video"
--设置大小
npcOneVideo.Size = Vector2.new(180, 130)
--设置位置
npcOneVideo.Position = Vector2.new(50, 50)
--设置图片路径
npcOneVideo.FileName = "res/video/login.mp4"
npcOneVideo.Loop = 1
```