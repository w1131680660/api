# Ray
------------------------------------------------------------------------------------------
## 描述

射线
注意：构造之后只读，对于实例中的 origin/Direction/Unit 进行修改是无意义的

------------------------------------------------------------------------------------------
## 属性
|<div style="width:700px">[Ray](/Api/DataType/Ray.md) &emsp;[<font color="dd00dd">New</font>]()</div>|
|:---|
|构造|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Origin</font>]()</div>|
|:---|
|射线起点|


|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Direction</font>]()</div>|
|:---|
|射线方向|


|<div style="width:700px">[Ray](/Api/DataType/Ray.md) &emsp;[<font color="dd00dd">Unit</font>]()</div>|
|:---|
|单位射线|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">ClosestPoint</font>]()</div>|
|:---|
|获取碰撞位置|

|<div style="width:700px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Distance</font>]()</div>|
|:---|
|射线距离|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:500px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">ClosestPoint</font> ]() ([Ray](/Api/DataType/Ray.md) ray, [Vector3](/Api/DataType/Vector3.md) point)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|射线某个方向投影的 <br>point = origin + cos(theta) *（unit）<br>（也表示点到射线的最先距离）||||
|**参数名称**|**类别**|**默认**|**描述**|
|ray|Ray|||
|point|[Vector3](/Api/DataType/Vector3.md)|||
|**返回类型**|||**概要**|
|[Vector3](/Api/DataType/Vector3.md)||||


|<div style="width:500px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">Distance</font> ]() ([Ray](/Api/DataType/Ray.md) ray, [Vector3](/Api/DataType/Vector3.md) point)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|射线到某个位置的距离||||
|**参数名称**|**类别**|**默认**|**描述**|
|ray|Ray|||
|point|[Vector3](/Api/DataType/Vector3.md)|||
|**返回类型**|||**概要**|
|[int](/Api/DataType/Number.md)|||距离|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local origin = Vector3.New(0,0,0)
local direct = Vector3.New(0,1,0)
local ray = Ray.New(origin, direct)
local unitRay = ray.Unit
local pos = Vector3.New(50,10,10)
local d = ray:Distance(pos)
local v3 = ray:ClosestPoint(pos)
print("Unit Ray:"..tostring(unitRay))
--Unit Ray:userdata: 42B65808
print("Ray Origin x:"..tostring(ray.Origin.x).." y:"..tostring(ray.Origin.y).." z:"..tostring(ray.Origin.z))
--Ray Origin x:0 y:0 z:0
print("Ray Direction x:"..tostring(ray.Direction.x).." y:"..tostring(ray.Direction.y).." z:"..tostring(ray.Direction.z))
--Ray Direction x:0 y:1 z:0
print("d:"..tostring(d))
--d:50.990196228027
print("v3:x:"..tostring(v3.x).." y:"..tostring(v3.y).." z:"..tostring(v3.z))
--v3:x:0 y:10 z:0
```