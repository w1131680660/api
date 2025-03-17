# GetOrderDataIndex

*所属类*:
* [CloudKVStore](/Api/Classes/Cloud/CloudKVStore.md)
------------------------------------------------------------------------------------------
## 描述

获取排行榜名次

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|bAscend|[bool](/Api/DataType/Bool.md)||是否上升|
|nIndex|[int](/Api/DataType/Number.md)||排行下标|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[int](/Api/DataType/Number.md)|排行榜名次 {key：uin value：排名，nick：昵称 }|
