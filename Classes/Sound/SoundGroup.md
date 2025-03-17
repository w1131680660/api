# SoundGroup

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">PlaySound</font> ()</div>|
|:---|
|播放/继续播放组内声音|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">StopSound</font> ()</div>|
|:---|
|停止播放组内声音|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ResumeSound</font> ()</div>|
|:---|
|重新播放组内声音（声音将从头开始播放）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">PauseSound</font> ()</div>|
|:---|
|暂停组内声音|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ChangeVolume</font>](/Api/Classes/Sound/SoundGroup_F/ChangeVolume.md) ([float](/Api/DataType/Number.md) value)</div>|
|:---|
|按比例改变组内声音音量（0~1），如：传入0.5会将组内Sound节点音量减半|

## 代码示例

```lua
--在WorkSpace下创建一个SoundGroup，并在添加两个音频子节点以及一个Script中填入一下脚本并运行
local soundgroup = script.Parent
soundgroup:PlaySound () --播放音效
wait(2)
soundgroup:ResumeSound() --重新播放音效
wait(2)
soundgroup:ChangeVolume(0.2) --控制音效声音
soundgroup:ResumeSound()
```