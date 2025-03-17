# FireClient 
-----------------------------------------------------------------------------------------
## 描述：

函数所属类：[RemotoEvent](/Api/Classes/Script/RemoteEvent.md)

为指定的玩家触发 [RemoteEvent.OnClientNotify](/Api/Classes/Script/RemoteEvent_F/OnClientNotify.md)。只有 [`LocalScript`](/Api/Classes/Script/LocalScript.md) 中在指定玩家的客户端上运行的连接会触发。与 [`RemoteFunction`](/Api/Classes/Script/RemoteFunction.md) 类的区别在于后者会队列请求。

因为此函数用于服务器向客户端通信，因此只能在 `Script` 内起效。

* 注意

    * 数据可以通过远程事件从服务器传递到客户端，就像数据从客户端传递到服务器一样。任何额外信息可作为 [RemoteEvent:FireClient](/Api/Class/Script/RemoteEvent_F/FireClient.md) 和 [FireAllClients](/Api/Classes/Script/RemoteEvent_F/FireAllClients.md) 函数的参数传递。注意 FireClient 函数仍需要将发送信息的目标玩家作为第一项参数来传递。

    * 有时游戏需要从一个客户端向另一个客户端发送信息。**MiniWorld Studio** 不支持客户端之间的直接联系，所以任何通信必须先经由服务器。这通常由远程事件完成（不过需要时也可以用函数）。首先，发送的客户端将调用 [FireServer](/Api/Class/Script/RemoteEvent_F/FireServer.md)。在服务器端，连接至 [OnServerNotify](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md) 的函数将监听到此触发，然后自身调用 [FireClient](/Api/Class/Script/RemoteEvent_F/FireClient.md)。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|uin      | [int](/Api/DataType/Number.md) ||被事件所影响的[Player](/Api/Classes/GamePlay/Player.md)的uin|
|argument    | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [RemoteEvent.OnServerNotify](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md) 方法的参数|


## 返回

无返回值

## 代码示例

```lua
print("1")

```