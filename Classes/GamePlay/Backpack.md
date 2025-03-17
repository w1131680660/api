# Backpack

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CoreUiEnabled</font></div>|
|:---|
|是否显示默认的快捷栏UI，默认值为false|

## 成员函数

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetTool</font>](/Api/Classes/GamePlay/Backpack_F/GetTool.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|获取某个键位对应的道具，index从1开始|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTool</font>](/Api/Classes/GamePlay/Backpack_F/SetTool.md) ([int](/Api/DataType/Number.md) index, [SandboxNode](/Api/Classes/Base/SandboxNode.md) tool)</div>|
|:---|
|设置道具到具体的物品栏按键位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveTool</font>](/Api/Classes/GamePlay/Backpack_F/RemoveTool.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|移除某物品栏道具|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetCurEquipedTool</font>](/Api/Classes/GamePlay/Backpack_F/GetCurEquipedTool.md) ()</div>|
|:---|
|获取当前装备的道具|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">FindTool</font>](/Api/Classes/GamePlay/Backpack_F/FindTool.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) tool)</div>|
|:---|
|查询道具是否已经放在物品栏中，返回下标|

