# ViewportPointToRay

*所属类*:
* [Camera](/Api/Classes/GamePlay/Camera.md)
------------------------------------------------------------------------------------------
## 描述

以朝向摄像机的方向，通过给定的距摄像机的深度，在视口上的某个位置创建单位射线（以像素为单位）

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|x|[float](/Api/DataType/Number.md)||x轴|
|y|[float](/Api/DataType/Number.md)||y轴|
|depth|[float](/Api/DataType/Number.md)||深度|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Ray](/Api/DataType/Ray.md)|Ray < 射线方向|
