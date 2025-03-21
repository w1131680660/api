# ScriptNode
------------------------------------------------------------------------------------------
## 描述

继承：[`SandboxNode`](/Api/Class/Script/SandboxNode.md)

------------------------------------------------------------------------------------------
## 属性


|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">luafile</font>]()</div>|
|:---|
|加载模式是`LoadMode::LUAFILE`时会执行设置的`luafile`的[`string`](/Api/DataType/String.md)内容|


|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">code</font>]()</div>|
|:---|
|加载模式是`LoadMode::LUACODE`时会执行设置`code`的字符串内容|

------------------------------------------------------------------------------------------
## 示例代码

```lua
--创建实例
local newScript = SandboxNode.New('ScriptNode')
--设置名字
newScript .Name = "my_script"
--设置脚本节点对应的文件
newScript.luafile = "res/jsonFiles/demo/SandboxNodeDemo.lua"
--设置脚本节点对应的string
newScript.code = "print('hello script')"
```