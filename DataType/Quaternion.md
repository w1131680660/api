# Quaternion
------------------------------------------------------------------------------------------
## 描述

四元数用于表示旋转。

四元数是实数{x，y，z，w}的四元组。四元数在数学上是欧拉角表示的一种方便的替代方法。可以在不经历万向节锁定的情况下对四元数进行插值。也可以使用四元数将一系列旋转使用到单个四元素中。

可以使用四元数相乘操作(Quaternion * (Quaterion / Vector3))，将旋转叠加起来，或者给3维坐标施加一个旋转。

一个四元数不能表示一次旋转超过180度（四元数会使用最短路径来表示旋转）

------------------------------------------------------------------------------------------
## 属性

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">New(float x, float y, float z, float w)</font></div>|
|:---|
|构造一个四元数，x,y,z,w必须满足四元数的基本规则，
```lua
-- 比如通过轴角(axis[归一化]-angle[弧度])来构造四元数
local x = axis.x * sin(angle / 2); 
local y = axis.y * sin(angle / 2); 
local z = axis.z * sin(angle / 2);
local w = cos(angle / 2);
```


|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">LookAt(Vector3 forward, Vector3 up)</font></div>|
|:---|
|通过指定forward方向和upward创建一个旋转, forward表示旋转之后的正前方方向，up表示旋转之后的正上方方向|
```lua
-- 创建一个旋转 (不旋转)
local valid, quat = Quaternion.LookAt(ZDir, YDir)
-- 创建一个旋转 (上下翻转-沿着z轴旋转180度)
valid, quat = Quaternion.LookAt(ZDir, 0 - YDir)
-- 创建一个旋转 (z轴转到x轴，旋转90度（左手螺旋定律，旋转九十度）)
valid, quat = Quaternion.LookAt(XDir, YDir)
```

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">FromEuler(float x, float y, float z)</font></div>|
|:---|
|使用欧拉角（角度）来构建一个四元数(旋转顺序是ZXY)|
```lua
local roll,yaw, pitch
local quat = Quaternion.FromEuler(pitch,yaw,roll)
```

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">FromAxisAngle(Vector3 axis, float angle)</font></div>|
|:---|
|通过轴角来构建一个四元数, angle是旋转角度（角度，非弧度）， axis旋转轴（需要归一化）|


|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">Lerp(Quaternion a, Quaternion b, float progress)</font></div>|
|:---|
|使用t控制a和b之间插值，然后对结果进行归一化|

------------------------------------------------------------------------------------------
## 函数
|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;[<font color="dd00dd">Lerp</font>](/Api/DataType/Quaternion_F/Lerp.md) ([Quaternion](/Api/DataType/Quaternion.md) a, [Quaternion](/Api/DataType/Quaternion.md) b, [float](/Api/DataType/Number.md) t)</div>|
|:---|
|通过t在a和b之间插值，然后对结果进行归一化|

| <div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;[<font color="dd00dd">RotateAxisAngle</font>](/Api/DataType/Quaternion_F/RotateAxisAngle.md) ([Vector3](/Api/DataType/Vector3.md) axis, [float](/Api/DataType/Number.md) angle)</div> |
| :----------------------------------------------------------- |
| 绕axis轴旋转angle角度                                        |

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">LookDir</font>](/Api/DataType/Quaternion_F/LookDir.md) ([Quaternion](/Api/DataType/Quaternion.md) targetq)</div>|
|:---|
|创建具有指定向前和向上方向的旋转|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">RotateToDir</font>](/Api/DataType/Quaternion_F/RotateToDir.md) ([Quaternion](/Api/DataType/Quaternion.md) target, [Quaternion](/Api/DataType/Quaternion.md) dir)</div>|
|:---|
|从from到to旋转一个旋转|

------------------------------------------------------------------------------------------
## 示例代码

```lua
-- ********* New *********
-- 创建一个四元数
local newq = Quaternion.New(0,0,2,1)
print("newq:"..tostring(newq))


-- ********* LookAt *********
-- 当前朝向
Vector3 relativePos = target.position - transform.position;
-- 头顶朝向(默认向上)  
local up = Vector3.New(0,1,0)
-- 使用指定的向前方向和向上方向转换成四元数                                
local b, rotation = Quaternion.LookAt(relativePos, up);
print("使用指定的向前方向和向上方向转换成四元数，转换是否成功:"..tostring(b))


-- ********* FromEuler *********
-- 绕y轴旋转30度（欧拉角转四元素）
Quaternion qfe = Quaternion.FromEuler(0, 30, 0);


-- ********* FromAxisAngle *********
-- 将变换的当前旋转设置为围绕y轴旋转30度的新旋转（Vector3.up）
local up = Vector3.New(0,1,0)
local rotation = Quaternion.FromAxisAngle(30, up);


-- ********* Lerp *********
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
local lerpRotation1 = Quaternion.Lerp(fromTf.rotation, toTf.rotation, timeCount * speed);
-- 或者
local newq = Quaternion.New(0,0,2,1)
local lerpRotation2 = newq:Lerp(fromTf.rotation, toTf.rotation, timeCount * speed);


-- ********* RotateAxisAngle *********
-- 设置旋转，使变换的y轴沿着全局y轴，变换的z轴沿着全局z轴
local newq = Quaternion.New(0,0,2,1)
local dir = Vector3.New(0,0,1)
local up = Vector3.New(0,1,0)
local angle = 0.01;  --角度
local rotation = newq:RotateAxisAngle(dir, up, angle);  -- return Quaternion


-- ********* LookDir *********
local newq = Quaternion.New(0,0,1,1)
local targetq = Quaternion.New(0,0,2,1)
local dir = newq:LookDir(targetq);   --return Vector3


-- ********* RotateToDir *********
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