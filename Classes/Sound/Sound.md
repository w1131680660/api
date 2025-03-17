# Sound

## 属性

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">SoundPath</font></div>|
|:---|
|声音资源路径|

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">Play</font></div>|
|:---|
|试听|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Volume</font></div>|
|:---|
|声音音量大小|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsLoop</font></div>|
|:---|
|该声音是否重复播放|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">PlayOnRemove</font></div>|
|:---|
|设置为true时，会在移除节点后播放一次声音|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">TransObject</font></div>|
|:---|
|设置为某个Transform节点后，Sound将在该节点的位置播放（3D声音），若Transform与FixPos均未设置，则为全局播放（2D声音）|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">FixPos</font></div>|
|:---|
|设置后，若没有指定Transform，则在指定位置(Vector3)播放3D声音|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsFixPosPlay</font></div>|
|:---|
|为true时代表正在FixPos属性所指位置播放3D声音|

|<div style="width:700px">[EnumRollOffMode](/Api/Enums/EnumRollOffMode.md) &emsp;<font color="dd00dd">RollOffMode</font></div>|
|:---|
|声音衰减模式，包括逆衰减（默认），线性衰减，线性平方衰减，锥型逆衰减模式|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RollOffMaxDistance</font></div>|
|:---|
|声音衰减最大距离|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RollOffMinDistance</font></div>|
|:---|
|声音衰减最小距离|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SoundPosition</font></div>|
|:---|
|声音播放位置（以毫秒为单位）|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">PlaySound</font> ()</div>|
|:---|
|播放/继续播放声音（调用后IsPlaying为true，IsPaused为false）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">StopSound</font> ()</div>|
|:---|
|停止播放声音（调用后IsPlaying为false）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ResumeSound</font> ()</div>|
|:---|
|重新播放声音（声音将从头开始播放）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">PauseSound</font> ()</div>|
|:---|
|暂停声音（调用后IsPaused为true）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SoundSyncMode</font> ()</div>|
|:---|
|设置同步模式|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">PlayFinish</font>](/Api/Classes/Sound/Sound_F/PlayFinish.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|Sound实例播放结束时触发该事件|

## 代码示例

```lua
local part = script.Parent --获取父节点
local sound = SandboxNode.new('Sound', part) --创建Sound节点
sound.SoundPath ="sandboxSysId://sounds/npc/chest.ogg" --设置资源路径
--sound.TransObject = script.Parent --绑定TransObject（播放3D声音）
sound.IsLoop = true --设置循环播放
--sound.PlayOnRemove = true --设置移除时播放
sound.RollOffMode = Enum.RollOffMode.Linear --设置声音衰减模式
sound.RollOffMinDistance = 300
sound.RollOffMaxDistance = 700
sound:PlaySound() --播放函数

--播放结束事件
sound.PlayFinish:connect(function(node)
	node:Destroy()
	print("sound is Destroy")
end)
```