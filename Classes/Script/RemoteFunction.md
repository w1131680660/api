# RemoteFunction


## 描述

**RemoteFunction**（远程函数）用于创建客户端和服务器用来彼此通信的游戏内`API`。开发者可以通过调用[`RemoteFunction`](/Api/Classes/Script/RemoteFunction.md)执行特定操作，并返回其结果。当不需要返回结果时，开发者应当转为使用异步调用且无需等待响应即可继续执行的[`RemoteEvent`](/Api/Classes/Script/RemoteEvent.md)。<br>

<font color=red>注意 RemoteFunction 对于调用方来说是同步执行的，会等待直到对端返回结果再执行下一条脚本。所以尽量不通过 OnClientInvoke 调用客户端</font>
* <font color=red>客户端如果报错，服务器同样会报错</font>
* <font color=red>如果客户端失去链接，同样会导致报错</font>
* <font color=red>如果客户端调用函数缺少返回值，则服务器会一直等待</font>


## 函数

|<div style="width:700px">[ReflexTuple](/Api/Parameter/Tuple.md)&emsp; [<font color="dd00dd">InvokeClient</font>](/Api/Classes/Script/RemoteFunction_F/InvokeClient.md)(&nbsp;[int](/Api/DataType/Number.md) client_uin ， [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|调用客户端的方法.<br>在客户端脚本 [LocalScript](/Api/Classes/Script/LocalScript.md) 中 设置 [`RemoteFunction:OnServerInvoke`](/Api/Classes/Script/RemoteFunction_F/OnServerInvoke.md) 为绑定至 `RemoteFunction` 的方法。   |

|<div style="width:700px">[ReflexTuple](/Api/Parameter/Tuple.md)&emsp; [<font color="dd00dd">InvokeServer</font>](/Api/Classes/Script/RemoteFunction_F/InvokeServer.md)(&nbsp;[ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:-----------------------|
|调用服务端的方法。<br>在服务端脚本 `Script` 中 设置[`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md) 为指定 `client` 调用绑定至 `RemoteFunction` 的方法。 |


## 回调

|<div style="width:700px">[ReflexTuple](/Api/Parameter/Tuple.md)&emsp;[<font color="dd00dd">OnServerInvoke</font>](/Api/Classes/Script/RemoteFunction_F/OnServerInvoke.md)( [int](/Api/DataType/Number.md) client_uin , [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:-----------------------|
|当服务器被[`RemoteFunction:InvokeServer`](/Api/Classes/Script/RemoteFunction_F/InvokeServer.md)调用时将对其进行调用。      |


|<div style="width:700px">[ReflexTuple](/Api/Parameter/Tuple.md)&emsp;[<font color="dd00dd">OnClientInvoke</font>](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md)( &nbsp;[ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:-----------------------|
|当客户端被[`RemoteFunction:InvokeClient`](/Api/Classes/Script/RemoteFunction_F/InvokeClient.md)调用时将对其进行调用。    |


## 示例代码

**脚本中创建RemoteFunction(注意要求其父节点必须是MainStorage)**

```lua
--代码中动态创建RemoteFunction示例 
local mainStorageService = game:GetService("MainStorage")
local node1 = SandboxNode.New('RemoteFunction')
node1.Name = "test_remotefunc_name"
node1:SetParent(mainStorageService)
```

* **`RemoteFunction:`客户端至服务器**

	当客户端希望使用远程函数时，将会通过[`LocalScript`](/Api/Classes/Script/LocalScript.md)内部的[`RemoteFunction:InvokeServer`](/Api/Classes/Script/RemoteFunction_F/InvokeServer.md)函数对服务器进行调用。<br>
	服务器会通过使用赋值操作符 =（而非`Script`中的事件）将函数绑定至[`RemoteFunction:OnServerInvoke`](/Api/Classes/Script/RemoteFunction_F/OnServerInvoke.md)的方法监听对[`InvokeServer`](/Api/Classes/Script/RemoteFunction_F/InvokeServer.md)函数的调用。当服务器被调用时，即会执行之前绑定的函数。

	```lua
	--客户端的调用脚本
	local mainStorageService = game:GetService("MainStorage")
	--这里的 testf1 是一个RemoteFunction类型的实例,它的name = "testf1"
	--都是预先在编辑地图时预先创建好的远程方法
	local testf1 = mainStorageService:WaitForChild("testf1")
	local ret = testf1:InvokeServer("ddddddddddabcdd")
	```

	```lua
	--服务端的监听执行脚本
	local mainStorageService = game:GetService("MainStorage")
	--这里的 testf1 是一个RemoteFunction类型的实例,它的name = "testf1"
	--都是预先在编辑地图时预先创建好的远程方法
	local testf1 = mainStorageService:WaitForChild("testf1")
	testf1.OnServerInvoke = function(uin, arg1)
	    print(" recv testf1  from client:"..tostring(uin).. " (arg1:) ".. tostring(arg1))
	    return "helloinvoke"
	end
	```

* **`RemoteFunction：`服务器至客户端**

	客户端的调用和服务器端的调用方法非常类似，但在调用客户端时需要将玩家uid作为参数传入。该过程所需要使用的函数为[`RemoteFunction:InvokeClient`](/Api/Classes/Script/RemoteFunction_F/InvokeClient.md)。<br>
	客户端通过使用赋值操作符 =（而非[`LocalScript`](/Api/Classes/Script/LocalScript.md)中的事件）将函数绑定至 [`RemoteFunction:OnClientInvoke`](/Api/Classes/Script/RemoteFunction_F/OnClientInvoke.md)的方法监听对[`InvokeClient`](/Api/Classes/Script/RemoteFunction_F/InvokeClient.md)函数的调用。当玩家（客户端）被调用时，即会执行之前绑定的函数。

	```
	--服务端的调用脚本
	--这里的 testf1 是一个RemoteFunction类型的实例,它的name = "testf1"
	--都是预先在编辑地图时预先创建好的远程方法
	local mainStorageService = game:GetService("MainStorage")
	local testf1 = mainStorageService:WaitForChild("testf1")
	local target_uin = 1000072593 --for test
	wait(1)
	local ret = testf1:InvokeClient( target_uin ,123,"invoke client")
	print(tostring(ret))
	```

	```
	--客户端的监听执行脚本
	--这里的 testf1 是一个RemoteFunction类型的实例,它的name = "testf1"
	--都是预先在编辑地图时预先创建好的远程方法
	local mainStorageService = game:GetService("MainStorage")
	local testf1 = mainStorageService:WaitForChild("testf1")

	testf1.OnClientInvoke = function(arg1, arg2)
	        print(" recv testf1  from server:"..tostring(arg1).. " (arg2:) ".. tostring(arg2))
	        return "onclientinvoke success"
	end
	```