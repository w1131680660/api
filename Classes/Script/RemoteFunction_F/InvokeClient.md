# InvokeClient
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[RemoteFunction](/Api/Classes/Script/RemoteFunction.md)

通过[`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md)将指定[Player](/Api/Classes/GamePlay/Player.md)客户端绑定至RemoteFunction，需要放至`Scirpt`中使用。

|当不需要放回结果，建议使用[RemotoEvent](/Api/Classes/Script/RemoteEvent.md)


- <font color="ff3333">注意：</font>
该函数会暂停调用的线程，直到结果被返回。如果客户端被服务器调用时中断或者网络连接失败，该函数则会出现错误，建议将该函数进行封装至pcall中。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|uin    | [Int](/Api/DataType/Int) ||需要绑定的 [Player](/Api/Classes/GamePlay/Player.md) uin|
|arguments    | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md) 方法的参数|


## 返回

|<div style="width:400px">类型</div>|<div style="width:400px">描述</div>|
|:--------------------|:--------------------|
|[ReflexTuple](/Api/DataType/tuple.md)   |[`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md)函数的返回值|

## 代码示例

```lua
print("1")

```