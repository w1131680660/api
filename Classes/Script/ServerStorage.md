# ServerStorage

*继承自*：
* [SandBoxNode](/Api/Classes/Base/SandboxNode.md)

## 描述

  其内容只能在服务器上访问的容器。 从 `ServerStorage` 继承的对象不会复制到客户端，也无法从 `LocalScripts` 访问。

  当脚本作为 `ServerStorage` 的父级时，脚本将不会运行，尽管可以访问和运行其中包含的 `ModuleScript` 。建议开发人员使用 `ServerScriptService` 来保存他们希望服务器执行的脚本。

  请注意，由于 `ServerStorage` 的内容只能由服务器访问，因此在客户端可以访问其内容之前，需要将其内容设置为其他地方（例如 `WorkSpace`）的父级。 建议需要服务器和客户端均可访问的容器的开发人员使用 `ReplicatedStorage`。

## 代码示例

```lua
local ServerStorage = game:GetService("ServerStorage")

local ROUND_TIME = 5

local map1 = Instance.New("Model")
map1.Name = "Map1"
map1.Parent = ServerStorage

local map2 = Instance.New("Model")
map2.Name = "Map2"
map2.Parent = ServerStorage

local map3 = Instance.New("Model")
map3.Name = "Map3"
map3.Parent = ServerStorage

local maps = { map1, map2, map3 }
while true do
  print("New map!")

  -- fetch new map
  local map = maps[1]
  currentMap.Parent = WorkSpace

  task.wait(ROUND_TIME)
end
```
