# AsyncHttpPost2

*所属类*：
* [NetService](/Api/Classes/Service/NetService.md)
------------------------------------------------------------------------------------------
## 描述

http异步post请求，带有callback

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|url|[string](/Api/DataType/String.md)||请求的url|
|postData|[string](/Api/DataType/String.md)||post请求参数|
|cb|[NetInstanceLuaCallback](/Api/DataType/NetInstanceLuaCallback.md)||lua回调函数|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[NetInstance](/Api/DataType/NetInstance.md)|lua异步post请求id|
