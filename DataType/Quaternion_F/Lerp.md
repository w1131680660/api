# Lerp

*所属类*：
* [Quaternion](/Api/DataType/Quaternion.md)
------------------------------------------------------------------------------------------
## 描述

通过t在a和b之间插值，然后对结果进行归一化

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|a|[Quaternion](/Api/DataType/Quaternion.md)||起始单位四元数值，当 t = 0 时返回|
|b|[Quaternion](/Api/DataType/Quaternion.md)||结束单位四元数值，当 t = 1 时返回。|
|t|[float](/Api/DataType/Number.md)||插值比。 该值被限制在 [0, 1] 范围内|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Quaternion](/Api/DataType/Quaternion.md)|返回一个四元素（在四元数 a 和 b 之间插值的单位四元数）|

------------------------------------------------------------------------------------------
## 示例代码

```lua
-- 目标旋转对象
local fromTf = SandboxNode.New('Transform')
fromTf:SetParent(workspace)
fromTf.Position = Vector3.New(100, 100, 100)  --设置全局位置
local toTf = SandboxNode.New('Transform')
toTf:SetParent(workspace)
toTf.Position = Vector3.New(50, 50, 50)

local speed = 0.01;
local timeCount = 0.0f;
local deltaTime = 1.0f
timeCount = timeCount + deltaTime;
local newq = Quaternion.New(0,0,2,1)
local lerpRotation2 = newq:Lerp(fromTf.rotation, toTf.rotation, timeCount * speed);
```