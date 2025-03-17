# SBXSignal
------------------------------------------------------------------------------------------
## 描述

`SBXSignal` 数据类型,（我们一般称之为`Event`事件）。其为用户定义的函数（我们称之为监听器）提供了一种在游戏中发生某些情况时调用的方法。 当事件发生时，`SBXSignal` 会触发并调用连接到它的任何监听器。 除此以外`SBXSignal` 还可以将参数传递给每个监听器以提供有关事件的额外信息。


## 函数

|<div style="width:700px">[SBXConnection](/Api/DataType/SBXConnection.md) &emsp;<font color="dd00dd">Connect</font>()</div>|
|:---|
|建立事件触发时要调用的函数。返回与连接关联的SBXConnection对象|

|<div style="width:700px">[SBXConnection](/Api/DataType/SBXConnection.md) &emsp;<font color="dd00dd">Emit</font>()</div>|
|:---|
|发送事件|

|<div style="width:700px">[SBXConnection](/Api/DataType/SBXConnection.md) &emsp;<font color="dd00dd">Wait</font>()</div>|
|:---|
|等待事件|

|<div style="width:700px">[SBXConnection](/Api/DataType/SBXConnection.md) &emsp;<font color="dd00dd">Clear</font>()</div>|
|:---|
|清空事件|


## 代码示例

```lua
--创建ui布局
local root = SandboxNode.New('UIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建按钮
local button= SandboxNode.New('UIButton', game.WorkSpace.uiroot)
button.Click:Connect(function(node,issuccess,mousepos) 
    print('you Clickme')
    print('Clickme pos:'..mousepos.x..' '..mousepos.y)
end)
```