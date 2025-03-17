# ModuleScript

*继承自*：
*  [`SandBoxNode`](/Api/Classes/Base/SandboxNode.md)

## 描述：

`ModuleScript`它只会运行一次，并且必定返回相同的一个值。然后在 `ModuleScriptNode`作为唯一参数的情况下，通过调用`require`返回此值。对于每个`Lua`环境，`ModuleScriptNode`运行且仅运行一次，并且在后续调用`require`时返回该相同的值。<br>

`ModuleScript`多用于重复方法的使用，在代码编写时，应当只编写一次，在其他地方对其调用。这样可以避免复写重复的函数方法，也可以将方法进行模块化管理。一般来`ModuleScript`用于集合一类方法或定义较为相近的方法。

需要注意的是，首次调用的时候不会暂停，直到获取到返回值。根据这种情况，一定要主要`ModuleScript`的嵌套问题，例如 **A(`ModuleScript`)** 对 **B(`ModuleScript`)** 进行了调用，但是 **B** 对 **A** 也进行了调用，则线程将挂起，但是不会暂停也不会报错，所以当出现复杂嵌套时，一定要注意`ModuleScript`之间相互的调用

## 示例代码：

在`WorkSpace`下创建一个`Script`脚本节点和`ModuleScript`脚本节点，填入对应内容

```lua
--ModuleScript
	local PrintFunction ={}

	function PrintFunction.Add(a,b)
		return a+b
	end

	function PrintFunction.pri(c)
		print(c)
	end

	return PrintFunction

```

```lua
--Script
	local fun= require(script.Parent.ModuleScript)

	Num = fun.Add(3,4)
	fun.pri(Num)

```