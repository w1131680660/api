# RemoteEvent

*继承自*：
*  [SandBoxNode](/Api/Classes/Base/SandboxNode.md)

## 描述
`RemoteEvent`（远程事件）的作用是在客户端和服务器端之间提供一个单向讯息传播途径，它允许`Script`（脚本）和[`LocalScript`](/Api/Classes/Script/LocalScript.md)（本地脚本）之间互相调用其内部的代码。讯息可以由客户端传向服务器端，也可以由服务器端传向特定的客户端，还可以由服务器端传给所有客户端。

为了让服务器端和客户端都能使用远程事件，`RemoteEvent`对象必须处于一个能让服务器端和客户端双方都能看到的位置，`RemoteEvent`要求存储在`MainStorage`里面。


## 函数

|<div style="width:700px">[void](/Api/DataType/Nil.md)&emsp; [<font color="dd00dd">FireServer</font>](/Api/Classes/Script/RemoteEvent_F/FireServer.md)(&nbsp;[ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|在服务器端用同样的参数触发[`RemoteEvent.OnServerNotify`](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md)事件，前面外加一个玩家参数。      |

|<div style="width:700px">[void](/Api/DataType/Nil.md)&emsp; [<font color="dd00dd">FireClient</font>](/Api/Classes/Script/RemoteEvent_F/FireClient.md)( [int](/Api/DataType/Number.md) uin , [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|为指定的玩家触发[`RemoteEvent.OnClientNotify`](/Api/Classes/Script/RemoteEvent_F/OnClientNotify.md)事件      |

|<div style="width:700px">[void](/Api/DataType/Nil.md)&emsp; [<font color="dd00dd">FireAllClients</font>](/Api/Classes/Script/RemoteEvent_F/FireAllClients.md)( [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|在每个客户端触发[`RemoteEvent.OnClientNotify`](/Api/Classes/Script/RemoteEvent_F/OnClientNotify.md)事件。      |

-----------------------------------------------------------------------------------------
## 事件(待定)

|<div style="width:700px">[Notify](/Api/Parameter/Notify.md)&emsp;[<font color="dd00dd">OnServerNotify</font>](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md)( [int](/Api/DataType/Number.md) client_uin , [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|当[`RemoteEvent.FireClient`](/Api/Classes/Script/RemoteEvent_F/FireClient.md)或[`RemoteEvent.FireAllClients`](/Api/Classes/Script/RemoteEvent_F/FireAllClients.md)从`Script`调用时触发[`LocalScript`](/Api/Classes/Script/LocalScript.md)内的监听函数。      |

|<div style="width:700px">[Notify](/Api/Parameter/Notify.md)&emsp;[<font color="dd00dd">OnClientNotify</font>](/Api/Classes/Script/RemoteEvent_F/OnClientNotify.md)( [ReflexTuple](/Api/Parameter/Tuple.md) arguments )</div>|
|:---------------------------------------------------------------------------------------|
|从一个[`LocalScript`](/Api/Classes/Script/LocalScript.md)中调用 [`RemoteEvent.FireServer`](/Api/Classes/Script/RemoteEvent_F/FireServer.md)时触发`Script`中的监听函数。      |


## 示例代码(待定)

* **脚本中创建RemoteEvent(注意要求其父节点必须是`MainStorage`)**

```lua
--代码中动态创建RemoteEvent示例 
local mainStorageService = game:GetService("MainStorage")
local node1 = SandboxNode.New('RemoteEvent')
node1.Name = "test_remoteevent_name"
node1:SetParent(mainStorageService)
```

* **`RemoteEvent：`服务器至多个客户端**
	
	通过远程事件，服务器能够以两种形式将消息发送给客户端：
	1. 服务器向单独指定客户端发送消息
	2. 服务器同时向所有客户端发送消息。

	如果要想将消息发送给所有客户端，在服务器内使用 [`RemoteEvent.FireAllClients`](/Api/Classes/Script/RemoteEvent_F/FireAllClients.md) 对所有客户端进行该事件的广播。需要注意的是，在此情况下无需将玩家作为参数进行传递（由于函数将为所有连接至服务器的客户端触发远程事件）。

  **如果需要监听此事件时，每个客户端都需要将函数连接至 OnClientNotify。**

	```lua
    --代码中动态创建RemoteEvent示例 
		local mainStorageService = game:GetService("MainStorage")
	local node1 = SandboxNode.New('RemoteEvent')
	node1.Name = "testnoargs"
	node1:SetParent(mainStorageService)
	--服务端的发送脚本
	local mainStorageService = game:GetService("MainStorage")
	--这里的testnoargs是一个RemoteEvent类型的实例,它的name = "testnoargs"
	--这里的testargs 是一个RemoteEvent类型的实例,它的name = "testargs "
	--都是预先在编辑地图时预先创建好的事件
	local testnoargs = mainStorageService:WaitForChild("testnoargs")
	local target_client_uin = 1000072589--for test
	testnoargs:fireClient( target_client_uin )

	local testargs   = mainStorageService:WaitForChild("testargs")
	testargs:fireAllClients(123,"abc")
	```

	```lua
	--客户端的监听脚本localScript
	local mainStorageService = game:GetService("MainStorage")

	--这里的testnoargs是一个RemoteEvent类型的实例,它的name = "testnoargs"
	--这里的testargs 是一个RemoteEvent类型的实例,它的name = "testargs "
	--都是预先在编辑地图时预先创建好的事件

	local testnoargs = mainStorageService:WaitForChild("testnoargs")

	testnoargs.OnClientNotify:Connect(function()
	    print("client recv testnoargs event from server")
	end)

	local testargs = mainStorageService:WaitForChild("testargs")
	testargs.OnClientNotify:Connect(function(arg1, arg2)
	    print("client recv testargs event from server:"..tostring(arg1)..tostring(arg2))
	end)
	```

* **`RemoteEvent：`客户端至服务器端**

	要想从客户端发送一条消息到服务器端，就需要在[`LocalScript`](/Api/Classes/Script/LocalScript.md)中执行函数[`RemoteEvent:FireServer`](/Api/Classes/Script/RemoteEvent_F/FireServer.md)。<br>
	与此同时，服务器端要监听通知[`OnServerNotify`](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md)。<br>
	当客户端调用[`FireServer`](/Api/Classes/Script/RemoteEvent_F/FireServer.md)函数时，所有订阅[`OnServerNotify`](/Api/Classes/Script/RemoteEvent_F/OnServerNotify.md)通知的服务器端的监听函数都会执行，注意这个过程不会立刻开始：过程的进展速度取决于客户端和服务器端之间的网络连接状况。<br>
	当从一个客户端向服务器端发送一个 `RemoteEvent` 的时候，可以自由携带参数。

	```lua
	--服务端的监听脚本
	local mainStorageService = game:GetService("MainStorage")

	--这里的testnoargs是一个RemoteEvent类型的实例,它的name = "testnoargs"
	--这里的testargs 是一个RemoteEvent类型的实例,它的name = "testargs "
	--都是预先在编辑地图时预先创建好的事件

	local testnoargs = mainStorageService:WaitForChild("testnoargs")

	testnoargs.OnServerNotify:Connect(function(uin)
	    print("server recv testnoargs event from client:"..tostring(uin))
	end)

	local testargs = mainStorageService:WaitForChild("testargs")
	testargs.OnServerNotify:Connect(function(uin, arg1, arg2)
	    print("server recv testargs event from client:"..tostring(uin),  tostring(arg1),tostring(arg2))
	end)
	```

	```lua
	----客户端的localScript脚本  向服务器发送远程事件
	wait(1)
	local mainStorageService = game:GetService("MainStorage")
	local testnoargs = mainStorageService:WaitForChild("testnoargs")        
	print("testnoargs:FireServer()")
	testnoargs:FireServer()
	wait(1)
	local testargs = mainStorageService:WaitForChild("testargs")        
	testargs:FireServer(1325,"abc")
	print("testargs:FireServer() arg1: 1325 arg2: abc")
	```