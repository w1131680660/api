# LookDir

*所属类*：
* [Quaternion](/Api/DataType/Quaternion.md)
------------------------------------------------------------------------------------------
## 描述

创建具有指定向前和向上方向的旋转

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|targetq|[Quaternion](/Api/DataType/Quaternion.md)||目标单位四元数值|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Vector3](/Api/DataType/Vector3.md)|朝向|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local newq = Quaternion.New(0,0,1,1)
local targetq = Quaternion.New(0,0,2,1)
local dir = newq:LookDir(targetq);   --return Vector3
```