# Team

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoAssignable</font></div>|
|:---|
|此属性用来决定加入游戏的Player是否允许自动分配到该队伍|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TeamColor</font></div>|
|:---|
|(ColorQuad)|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerAdded</font>](/Api/Classes/GamePlay/Team_F/PlayerAdded.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|新增一个玩家|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerRemoved</font>](/Api/Classes/GamePlay/Team_F/PlayerRemoved.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|移除一个玩家|

## 代码示例

```lua
local Teams = game:GetService('Teams')
--创建开始队伍
local team1 = SandboxNode.new('Team', Teams)
team1.AutoAssignable = true
Teams.TeamColor = Vector3.new(255, 0, 0)
```