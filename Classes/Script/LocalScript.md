# LocalScript

*继承自*：
* [SandBoxNode](/Api/Classes/Base/SandboxNode.md)

## 描述

[`LocalScript`](/Api/Classes/Script/LocalScript.md)是用于客机运行Lua代码的容器，它作用于仅在客户端的对象，例如玩家的[Camera](/Api/Classes/GamePlay/Camera.md)。通过[Players](/Api/Classes/GamePlay/Players.md)获得的[`LocalPlayer`](/Api/Classes/GamePlay/LocalPlayer.md)为当前运行该脚本的玩家

[`LocalScript`](/Api/Classes/Script/LocalScript.md)仅在以下环境下才可运行:

* [`Player`](/Api/Classes/GamePlay/Player.md) 的 [`Backpack`](/Api/Classes/GamePlay/Backpack.md)，如 [`Tool`](/Api/Classes/GamePlay/Tool.md) 的子项

* [`Player`](/Api/Classes/GamePlay/Player.md) 的 [`Actor`](/Api/Classes/Role/Actor.md) 模型

* [`Player`](/Api/Classes/GamePlay/Player.md) 的 `PlayerGui`

* [`Player`](/Api/Classes/GamePlay/Player.md) 的 `PlayerScripts`

* `LocalFirst` 服务


## 代码示例

使用`LocalScript`写入代码后，仅在*描述*中所说位置会打印 *Hello world!*

```lua
print("Hello world!") --使用
```
