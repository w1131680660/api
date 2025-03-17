# StarterPlayerScripts

*继承自*：
* [SandboxNode](/Api/Classes/Base/SandboxNode.md)

## 描述

`StarterPlayerScripts` 是位于 `StarterPlayer` 服务内的容器对象。 它包含 `LocalScripts` 和其他对象，当玩家加入游戏时，这些对象将被复制到 `PlayerScripts` 容器中。 例如，如果您想在满足某些条件时在客户端上创建特殊效果，您可以在该对象中放置一个 `LocalScript` 来实现此目的。

该对象也是使用 `ContextActionService` 定义附加输入的 `LocalScript` 的好地方。 对于仅在玩家生成时相关的输入，您可以在 `Players.LocalPlayer` 角色生成时使用 `ContextActionService:BindAction()`。 然后，当它们死亡或消失时，使用 `ContextActionService:UnbindAction()`。
