# Model2D

## 属性

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Size</font></div>|
|:---|
|模型的包围盒大小|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Center</font></div>|
|:---|
|模型的中心点所在世界坐标|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TextureId</font></div>|
|:---|
|设置模型的材质，即资源id|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">Color</font></div>|
|:---|
|模型的颜色|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableGravity</font></div>|
|:---|
|是否开启重力|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Anchored</font></div>|
|:---|
|是否锚定|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Gravity</font></div>|
|:---|
|重力|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Mass</font></div>|
|:---|
|密度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Density</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Restitution</font></div>|
|:---|
|弹性|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Friction</font></div>|
|:---|
|马擦力|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Velocity</font></div>|
|:---|
|速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">AngleVelocity</font></div>|
|:---|
|角速度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanCollide</font></div>|
|:---|
|是否可以产生物理碰撞|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanTouch</font></div>|
|:---|
|是否可以碰撞回调|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GroupID</font></div>|
|:---|
|设置碰撞组|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnablePhysics</font></div>|
|:---|
|是否生效|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableCCD</font></div>|
|:---|
|会影响性能，所以默认不开启|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableDrawCollider</font></div>|
|:---|
||

|<div style="width:700px">[PHYSX2D_TYPE](/Api/Enums/PHYSX2D_TYPE.md) &emsp;<font color="dd00dd">PhysXType</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">FlippedX</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">FlippedY</font></div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Touched</font>](/Api/Classes/Other/Model2D_F/Touched.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [Vector2](/Api/DataType/Vector2.md) pos, [Vector2](/Api/DataType/Vector2.md) normal)</div>|
|:---|
|模型被其他模型碰撞时，会触发一个Touched通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TouchEnded</font>](/Api/Classes/Other/Model2D_F/TouchEnded.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|模型被其他模型碰撞结束时，会触发一个TouchEnded通知|

