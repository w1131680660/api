# StarterGui

*继承自*：

* [Service](/Api/Classes/Service/Service.md)

## 描述

  全局服务节点，提供通用服务节点的基类。注：设置父节点必须是`GameNode`

  `StarterGui` 服务是一个容器对象，旨在保存 `GUI` 对象（例如 `ScreenGuis`）。

  `StarterGui` 作为容器
  当 `Player.Character` 重生时，其 `PlayerGui` 的内容将被清空。 然后，`StarterGui` 的子级及其后代将被复制到 `PlayerGui` 中。

  GUI 对象只会被放置到每个 Player 的 PlayerGui 中一次，并且在 Player 重生时不会被删除。

  StarterGui 作为界面
  StarterGui 还包括一系列允许您与 CoreGui 交互的功能。 可用于禁用 CoreGui 的元素。 StarterGui:SetCore() 可以执行一系列功能，包括创建通知和系统消息。

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsRockerEnable</font></div>|
|:---|
|摇杆是否启用|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">WalkZone</font></div>|
|:---|
|步行区|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BackGroundIcon</font></div>|
|:---|
|背景图标|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">DotIcon</font></div>|
|:---|
|点图标|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DotScale</font></div>|
|:---|
|点比例|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">InactiveAlpha</font></div>|
|:---|
|透明度是否激活|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Alpha</font></div>|
|:---|
|透明度|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">RockerPosition</font></div>|
|:---|
|摇杆位置|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">RockerSize</font></div>|
|:---|
|摇杆尺寸|

|<div style="width:700px">[ScaleType](/Api/Enums/ScaleType.md) &emsp;<font color="dd00dd">BackGroundScaleType</font></div>|
|:---|
|背景比例尺类型|

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">BackGroundSliceCenter</font></div>|
|:---|
|背景切片中心|

|<div style="width:700px">[ScaleType](/Api/Enums/ScaleType.md) &emsp;<font color="dd00dd">DotScaleType</font></div>|
|:---|
|点刻度类型|

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">DotSliceCenter</font></div>|
|:---|
|点切片中心|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">JumpIcon</font></div>|
|:---|
|跳转图标|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">JumpIconShow</font></div>|
|:---|
|跳转图标显示|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyRockerChange</font>](/Api/Classes/Other/StarterGui_F/NotifyRockerChange.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|摇杆切换会触发一个事件|

## 代码示例


```lua
local StarterGui = game:GetService("StarterGui")
```
