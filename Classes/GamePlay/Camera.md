# Camera

## 属性

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">PickPosition</font></div>|
|:---|
|摄像机跟随鼠标在游戏内指向的三维坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LookFocus</font></div>|
|:---|
|摄像机焦点，镜头所看向的点|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ZNear</font></div>|
|:---|
|摄像机的近平面|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ZFar</font></div>|
|:---|
|摄像机的远平面|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FieldOfView</font></div>|
|:---|
|设置摄像机垂直视野的角度|

|<div style="width:700px">[CameraType](/Api/Enums/CameraType.md) &emsp;<font color="dd00dd">CameraType</font></div>|
|:---|
|摄像机类型|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;<font color="dd00dd">CameraSubject</font></div>|
|:---|
|摄像机子节点|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ViewportSize</font></div>|
|:---|
|描述客户端视口的尺寸（以像素为单位）|

## 成员函数

|<div style="width:700px">[Ray](/Api/DataType/Ray.md) &emsp;[<font color="dd00dd">ViewportPointToRay</font>](/Api/Classes/GamePlay/Camera_F/ViewportPointToRay.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) depth)</div>|
|:---|
|以朝向摄像机的方向，通过给定的距摄像机的深度，在视口上的某个位置创建单位射线（以像素为单位）|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">WorldToViewportPoint</font>](/Api/Classes/GamePlay/Camera_F/WorldToViewportPoint.md) ([Vector3](/Api/DataType/Vector3.md) position)</div>|
|:---|
|将一个世界坐标position转换到摄像机视口坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">WorldToUIPoint</font>](/Api/Classes/GamePlay/Camera_F/WorldToUIPoint.md) ([Vector3](/Api/DataType/Vector3.md) position)</div>|
|:---|
|将3D节点世界坐标position转UI节点坐标|

## 代码示例

```lua
--创建相机
local camera = SandboxNode.new('Camera')
local workSpace = game.WorkSpace
--设置父节点
camera:SetParent(workSpace)
--设置视角大小
camera.FieldOfView = 100.0
--设置相机位置
camera.Position = Vector3.new(500, 700, 500)
```