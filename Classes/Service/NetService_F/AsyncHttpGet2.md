# AsyncHttpGet2

*所属类*：
* [NetService](/Api/Classes/Service/NetService.md)
------------------------------------------------------------------------------------------
## 描述

http异步get请求，带有callback

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|url|[string](/Api/DataType/String.md)||请求的url|
|cb|[NetInstanceLuaCallback](/Api/DataType/NetInstanceLuaCallback.md)||lua回调函数|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[NetInstance](/Api/DataType/NetInstance.md)|lua异步get请求id|
