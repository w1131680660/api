# RotateAxisAngle

*所属类*：
* [Quaternion](/Api/DataType/Quaternion.md)
------------------------------------------------------------------------------------------
## 描述

绕axis轴旋转angle角度

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|axis|[Vector3](/Api/DataType/Vector3.md)||轴方向|
|angle|[float](/Api/DataType/Number.md)||旋转角度|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Quaternion](/Api/DataType/Quaternion.md)||

------------------------------------------------------------------------------------------
## 示例代码

```lua
-- 设置旋转，使变换的y轴沿着全局y轴，变换的z轴沿着全局z轴
local newq = Quaternion.New(0,0,2,1)
local up = Vector3.New(0,1,0) -- 头顶朝向(默认向上) 
local angle = 180;  --角度
local rotation = newq:RotateAxisAngle(up, angle);  -- return Quaternion
```