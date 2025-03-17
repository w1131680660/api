# SBXConnection
------------------------------------------------------------------------------------------
## 描述

`SBXConnection`数据类型，也称为`Connection`，是由事件 [SBXSignal](/Api/DataType/SBXSignal.md) 的`Connect`方法返回的一个特殊对象。这主要用于断开监听器与 [SBXSignal](/Api/DataType/SBXSignal.md) 的连接。

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsConnected</font></div>|
|:---|
|判断与事件是否还有连接|

## 函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Disconnect</font>()</div>|
|:---|
|断开与事件的连接|


## 代码示例

```lua
local root = SandboxNode.New('UIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建按钮
local button= SandboxNode.New('UIButton', game.WorkSpace.uiroot)
local connection = button.Click:Connect(function(node,issuccess,mousepos) 
    print('you Clickme')
    print('Clickme pos:'..mousepos.x..' '..mousepos.y)
end)

wait(5)
connection:Disconnect()
print("Event has been disconnected")
```