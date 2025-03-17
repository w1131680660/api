# PickObjects

*所属类*:
* [UserInputService](/Api/Classes/Input/UserInputService.md)
------------------------------------------------------------------------------------------
## 描述

从给定的obj列表中，根据传入的2D屏幕坐标，拾取指定对象

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|mouseX|[float](/Api/DataType/Number.md)||鼠标在2D屏幕的x坐标|
|mouseY|[float](/Api/DataType/Number.md)||鼠标在2D屏幕的y坐标|
|objects|[table](/Api/DataType/Table.md)||给定的游戏对象列表|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[SandboxNode](/Api/Classes/Base/SandboxNode.md)|单个游戏对象|
