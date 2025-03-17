# SoundService

## 属性

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RolloffScale</font></div>|
|:---|
|3D声音衰减速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DistanceFactor</font></div>|
|:---|
|3D声音衰减距离|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DopplerScale</font></div>|
|:---|
|3D声音多普勒效应强度|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GlobalVolume</font></div>|
|:---|
|全局音量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MusicOpen</font></div>|
|:---|
|打开游戏内背景音乐|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetListener</font>](/Api/Classes/Sound/SoundService_F/SetListener.md) ([ListenerType](/Api/Enums/EnumListenerType.md) type, [SandboxNode](/Api/Classes/Base/SandboxNode.md) object)</div>|
|:---|
|设置监听类型与监听者|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">PlayerLocalSound</font>](/Api/Classes/Sound/SoundService_F/PlayerLocalSound.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) sound)</div>|
|:---|
|在本地播放声音（2D，不会同步）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSoundOpen</font>](/Api/Classes/Sound/SoundService_F/SetSoundOpen.md) ([bool](/Api/DataType/Bool.md) value)</div>|
|:---|
|在本地开关声音（包括游戏本身的声音节点）|

## 代码示例

```lua
local SoundService = game:GetService("SoundService")
SoundService:SetSoundOpen(true)                    --打开声音
local listenertype = SoundService.ListenerType     --监听类型
local listenerobject = SoundService.ListenerObject --监听对象
SoundService.RolloffScale = 1                      --衰减速度
SoundService.DistanceFactor = 0                    --衰减距离
SoundService.DopplerScale = 0                      --多普勒效应强度
local soundnode = game.WorkSpace.Sound             --获取Sound节点
SoundService:PlayerLocalSound(soundnode)           --本地播放
local transnode = game.WorkSpace.TransNode         --获取Transfrom节点
SoundService:SetListener(Enum.ListenerType.TransObject,transnode)       --设置监听者
```