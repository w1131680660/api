# RotateToDir

*所属类*：
* [Quaternion](/Api/DataType/Quaternion.md)
------------------------------------------------------------------------------------------
## 描述

从from到to旋转一个旋转

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|target|[Quaternion](/Api/DataType/Quaternion.md)||目标单位四元数值，当 t = 0 时返回|
|dir|[Quaternion](/Api/DataType/Quaternion.md)||起始单位四元数值，当 t = 1 时返回。|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Vector3](/Api/DataType/Vector3.md)|朝向|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game.WorkSpace
-- 目标旋转对象
local targetTf = SandboxNode.New('Transform')
targetTf:SetParent(workspace)
targetTf.Position = Vector3.New(100, 100, 100)  --设置全局位置

local transform = SandboxNode.New('Transform')
transform:SetParent(workspace)
transform.Position = Vector3.New(50, 50, 50)

local newq = Quaternion.New(0,0,0,1)
local dir = newq:RotateToDir(transform.Rotation, targetTf.Rotation);  --return Vector3
```