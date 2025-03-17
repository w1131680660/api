# LegacyAnimation

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnablePlayEvent</font></div>|
|:---|
|是否开启播放事件|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Classes/Animation/LegacyAnimation_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了|

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;[<font color="dd00dd">GetAnimationIDs</font>](/Api/Classes/Animation/LegacyAnimation_F/GetAnimationIDs.md) ()</div>|
|:---|
|获取动画ID|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetAnimationPriority</font>](/Api/Classes/Animation/LegacyAnimation_F/GetAnimationPriority.md) ([int](/Api/DataType/Number.md) seqid)</div>|
|:---|
|获取动画优先级|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAnimationPriority</font>](/Api/Classes/Animation/LegacyAnimation_F/SetAnimationPriority.md) ([int](/Api/DataType/Number.md) seqid, [int](/Api/DataType/Number.md) value)</div>|
|:---|
|设置动画优先级|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetAnimationWeight</font>](/Api/Classes/Animation/LegacyAnimation_F/GetAnimationWeight.md) ([int](/Api/DataType/Number.md) seqid)</div>|
|:---|
|获取动画权重|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAnimationWeight</font>](/Api/Classes/Animation/LegacyAnimation_F/SetAnimationWeight.md) ([int](/Api/DataType/Number.md) seqid, [float](/Api/DataType/Number.md) value)</div>|
|:---|
|设置动画权重|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Play</font>](/Api/Classes/Animation/LegacyAnimation_F/Play.md) ([int](/Api/DataType/Number.md) id, [float](/Api/DataType/Number.md) speed, [int](/Api/DataType/Number.md) loop)</div>|
|:---|
|播放动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">PlayEx</font>](/Api/Classes/Animation/LegacyAnimation_F/PlayEx.md) ([int](/Api/DataType/Number.md) id, [float](/Api/DataType/Number.md) speed, [int](/Api/DataType/Number.md) loop, [int](/Api/DataType/Number.md) priority, [float](/Api/DataType/Number.md) weight)</div>|
|:---|
|播放动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Stop</font>](/Api/Classes/Animation/LegacyAnimation_F/Stop.md) ([int](/Api/DataType/Number.md) id)</div>|
|:---|
|停止动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">StopEx</font>](/Api/Classes/Animation/LegacyAnimation_F/StopEx.md) ([int](/Api/DataType/Number.md) id, [bool](/Api/DataType/Bool.md) reset)</div>|
|:---|
|停止动画|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">StopAll</font>](/Api/Classes/Animation/LegacyAnimation_F/StopAll.md) ([bool](/Api/DataType/Bool.md) reset)</div>|
|:---|
|停止所有动画|

## 事件

