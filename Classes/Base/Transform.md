# Transform

## 属性

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|全局坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Euler</font></div>|
|:---|
|全局欧拉角|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Euler</font></div>|
|:---|
|全局欧拉角|

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;<font color="dd00dd">Rotation</font></div>|
|:---|
|全局旋转|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LocalPosition</font></div>|
|:---|
|局部坐标|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LocalEuler</font></div>|
|:---|
|局部欧拉角|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LocalEuler</font></div>|
|:---|
|局部欧拉角|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CubeBorderEnable</font></div>|
|:---|
|立方体边框是否被禁止|

|<div style="width:700px">[LayerIndexDesc](/Api/Enums/LayerIndexDesc.md) &emsp;<font color="dd00dd">Layer</font></div>|
|:---|
|灯光层级|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">ForwardDir</font></div>|
|:---|
|看向指定方向|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">InheritParentVisible</font></div>|
|:---|
|是否跟随父节点显示或者隐藏，不影响visible属性|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Locked</font></div>|
|:---|
|是否场景操作选中|

## 成员函数

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">GetRenderPosition</font>](/Api/Classes/Base/Transform_F/GetRenderPosition.md) ()</div>|
|:---|
|获取渲染世界位置|

|<div style="width:700px">[Quaternion](/Api/DataType/Quaternion.md) &emsp;[<font color="dd00dd">GetRenderRotation</font>](/Api/Classes/Base/Transform_F/GetRenderRotation.md) ()</div>|
|:---|
|获取渲染世界旋转|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">GetRenderEuler</font>](/Api/Classes/Base/Transform_F/GetRenderEuler.md) ()</div>|
|:---|
|获取渲染世界欧拉角|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLocalPosition</font>](/Api/Classes/Base/Transform_F/SetLocalPosition.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置本地位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLocalScale</font>](/Api/Classes/Base/Transform_F/SetLocalScale.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置本地缩放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLocalEuler</font>](/Api/Classes/Base/Transform_F/SetLocalEuler.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置本地欧拉角|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetWorldPosition</font>](/Api/Classes/Base/Transform_F/SetWorldPosition.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置全局位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetWorldScale</font>](/Api/Classes/Base/Transform_F/SetWorldScale.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置全局缩放|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetWorldEuler</font>](/Api/Classes/Base/Transform_F/SetWorldEuler.md) ([float](/Api/DataType/Number.md) x, [float](/Api/DataType/Number.md) y, [float](/Api/DataType/Number.md) z)</div>|
|:---|
|设置全局欧拉角|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">LookAt</font>](/Api/Classes/Base/Transform_F/LookAt.md) ([Vector3](/Api/DataType/Vector3.md) x, [bool](/Api/DataType/Bool.md) y)</div>|
|:---|
|看向指定位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">LookAtObject</font>](/Api/Classes/Base/Transform_F/LookAtObject.md) ([SceneTransObject*](/Api/Enums/SceneTransObject*.md) x, [bool](/Api/DataType/Bool.md) y)</div>|
|:---|
|看向指定位置|

## 代码示例

```lua
local trans = SandboxNode.new('Transform')
local workSpace = game.WorkSpace
trans:SetParent(workSpace)
--设置全局位置
trans.Position = Vector3.new(100, 100, 100)
--设置局部大小
trans.LocalScale = Vector3.new(20, 1, 1)
```