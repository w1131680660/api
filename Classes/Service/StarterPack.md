# StarterPack

*继承自*：

* [Service](/Api/Classes/Service/Service.md)

## 描述

  一个服务级容器，当玩家生成时，其内容会被复制到每个玩家的背包中。 它一般用来存放`Tools`，但有时也用来存放`LocalScripts`，以确保每个玩家都得到一份副本。

  当玩家的角色生成时，`StarterPack` 及其 `StarterGear` 的内容将被复制到他们的背包中。 一旦角色死亡，背包就会被移除并创建一个新背包——使用 `StarterPack` 和 `StarterGear` 的内容填充它。

  `StarterPack` 用于确定所有玩家生成时都会使用的一组工具。 如果开发人员想要确保某些工具可供特定玩家使用，那么他们需要将这些工具直接设置为玩家的背包的父级。

  注意：虽然 `StarterPack` 的内容通常是预定义的，但可以在游戏运行时通过相应地添加和删除工具来更改内容。 当玩家重生并重新加载背包时，这些更新将传递到玩家的背包上。 对 `StarterPack` 的更改应由服务器进行。


## 代码示例

```lua
-- 可以使用以下代码将工具添加到 StarterPack。
Tool.Parent = game:GetService("StarterPack")
```
