# InvokeServer
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[RemoteFunction](/Api/Classes/Script/RemoteFunction.md)

该函数用于客户端对服务器的调用，因为服务器内存储了许多客户端没有的信息，且部分游戏操作必须在服务端内进行。

该函数被调用后，。通过对[RemoteFunction](/Api/Classes/Script/RemoteFunction.md)绑定这只RemoteFunction获取其返回值。该函数需要在[LocalScript](/Api/Classes/Script/LocalScript.md)中运行

|当不需要放回结果，建议使用[RemotoEvent](/Api/Classes/Script/RemoteEvent.md)


- <font color="ff3333">注意：</font>
该函数会暂停调用的线程，直到结果被返回。与 [InvokeClient](/Api/Classes/Script/RemoteFunction_F/InvokeClient.md)相比，默认清空下可不传递参数进行使用

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|arguments    | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md) 方法的参数|


## 返回

|<div style="width:400px">类型</div>|<div style="width:400px">描述</div>|
|:--------------------|:--------------------|
|[ReflexTuple](/Api/DataType/tuple.md)   |[`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md)函数的返回值|

## 代码示例

```lua
print("1")

```