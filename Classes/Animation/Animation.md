# Animation

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Classes/Animation/Animation_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的资源|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsPlaying</font>](/Api/Classes/Animation/Animation_F/IsPlaying.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|是否正在播放某个切片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Stop</font>](/Api/Classes/Animation/Animation_F/Stop.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|停止某个动画切片播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSpeed</font>](/Api/Classes/Animation/Animation_F/SetSpeed.md) ([string](/Api/DataType/String.md) name, [float](/Api/DataType/Number.md) speed)</div>|
|:---|
|设置某个动画切片播放速度|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Rewind</font>](/Api/Classes/Animation/Animation_F/Rewind.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|设置某个动画从头开始播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetWrapMode</font>](/Api/Classes/Animation/Animation_F/SetWrapMode.md) ([string](/Api/DataType/String.md) name, [WrapMode](/Api/Enums/AnimationWrapMode.md) wrap)</div>|
|:---|
|设置某个动画切片wrap模式（动画边缘处理）|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetClips</font>](/Api/Classes/Animation/Animation_F/GetClips.md) ()</div>|
|:---|
|获取当前animation持有的所有动画切片资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetClips</font>](/Api/Classes/Animation/Animation_F/SetClips.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) assets)</div>|
|:---|
|设置当前animation持有的动画切片资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateClips</font>](/Api/Classes/Animation/Animation_F/UpdateClips.md) ([AssetResType](/Api/Enums/AssetResType.md) resType, [table](/Api/DataType/Table.md) urls)</div>|
|:---|
|更新动画切片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetDefaultClip</font>](/Api/Classes/Animation/Animation_F/SetDefaultClip.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|设置默认动画切片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateDefaultClip</font>](/Api/Classes/Animation/Animation_F/UpdateDefaultClip.md) ([AssetResType](/Api/Enums/AssetResType.md) resType, [string](/Api/DataType/String.md) url)</div>|
|:---|
|更新默认动画切片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Play</font>](/Api/Classes/Animation/Animation_F/Play.md) ([string](/Api/DataType/String.md) name, [PlayMode](/Api/Enums/AnimationPlayMode.md) playMode)</div>|
|:---|
|播放切片|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Blend</font>](/Api/Classes/Animation/Animation_F/Blend.md) ([string](/Api/DataType/String.md) name, [float](/Api/DataType/Number.md) targetWeight, [float](/Api/DataType/Number.md) time)</div>|
|:---|
|设置切片动画混合权重|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">CrossFade</font>](/Api/Classes/Animation/Animation_F/CrossFade.md) ([string](/Api/DataType/String.md) name, [float](/Api/DataType/Number.md) targetWeight, [PlayMode](/Api/Enums/AnimationPlayMode.md) playMode)</div>|
|:---|
|设置切片动画渐变（fade）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AddClip</font>](/Api/Classes/Animation/Animation_F/AddClip.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [string](/Api/DataType/String.md) name, [int](/Api/DataType/Number.md) firstFrame, [int](/Api/DataType/Number.md) lastFrame, [bool](/Api/DataType/Bool.md) loop)</div>|
|:---|
|添加一个切片动画|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateClip</font>](/Api/Classes/Animation/Animation_F/UpdateClip.md) ([AssetResType](/Api/Enums/AssetResType.md) resType, [string](/Api/DataType/String.md) url, [string](/Api/DataType/String.md) name, [int](/Api/DataType/Number.md) firstFrame, [int](/Api/DataType/Number.md) lastFrame, [bool](/Api/DataType/Bool.md) loop)</div>|
|:---|
|更新一个切片动画|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveClip</font>](/Api/Classes/Animation/Animation_F/RemoveClip.md) ([string](/Api/DataType/String.md) clipname)</div>|
|:---|
|按名称移除一个动画切片|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetAutoPlay</font>](/Api/Classes/Animation/Animation_F/GetAutoPlay.md) ()</div>|
|:---|
|获取是否自动播放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAutoPlay</font>](/Api/Classes/Animation/Animation_F/SetAutoPlay.md) ([bool](/Api/DataType/Bool.md) autoPlay)</div>|
|:---|
|设置自动播放|

