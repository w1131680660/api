# Script

*继承自*：
* [SandBoxNode](/Api/Classes/Base/SandboxNode.md)

## 描述

`Script`是一个 `Lua` 代码容器，可以访问服务器端对象、属性和事件，例如向玩家授予徽章，而客户端上的 `LocalScript` 则不能。

一旦满足以下条件，脚本代码就会在新线程中运行：

其 `Enabled` 属性为 `true`。
`Script` 对象是 `Workspace` 或 `ServerScriptService` 的后代。
该脚本将继续运行，直到不满足上述条件、终止或引发错误（除非该错误是由连接到正在触发的某个事件的函数引发的）。 此外，如果脚本或其祖先之一被破坏，线程将停止。 即使 `Parent` 属性设置为 `nil`，脚本也将继续运行，并且脚本不会被销毁。


## 代码示例

```lua
-- 某个挂载在UIButton下的子脚本如何获取父类（UIButton）
local button = script.Parent

button.Click:Connect(function(node,issuccess,mousepos) 
    print('you Clickme')
    print('Clickme pos:'..mousepos.x..' '..mousepos.y)
end)
```