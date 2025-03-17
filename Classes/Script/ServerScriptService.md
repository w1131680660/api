# ServerScriptService

*继承自*：
* [SandBoxNode](/Api/Classes/Base/SandboxNode.md)


## 描述

  服务器脚本服务。用来存放服务器脚本，并且会优先执行，不会将子节点同步到客户端，相应的子节点如果有 `LocalScript` 也不会执行。

  `ServerScriptService` 是 `Script`、`ModuleScript` 和其他脚本相关资产的容器服务，仅供服务器使用。内容根本不会复制到玩家客户端，这允许安全存储重要的游戏逻辑。 如果脚本对象在此服务内且未禁用，则它们将运行。

  在 `ServerScriptService` 中运行的脚本可能需要访问与脚本无关的各种其他资产，例如要克隆的预制模型。 此类资产应放入 `ServerStorage` 中，其行为与此服务类似，只是脚本对象即使未禁用也不会运行。 
<!--   对服务器和客户端都有用的资产和 `ModuleScript` 应该放在 `ReplicatedStorage` 中。 最后，您可以通过使用文件夹进一步组织该服务中的对象，而不会影响其行为方式。 -->



