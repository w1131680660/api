# LuaTable

------------------------------------------------------------------------------------------
## 描述

`Table`（表）为可以储存多个值的 `Lua` 数据类型，其中包括数字、布尔值、字符串、函数等多种类型。表的构造使用中括号`({ })`，如下所示：

```lua
-- 构建一个分配至变量“t”的空表
local t = {}
print(t)
```

  >表格在构建后即可用作数组或字典，如以下各部分中所述。

------------------------------------------------------------------------------------------
## 数组

数组是一组简单的有序值，可用于存储数据集合，例如一组拥有相同道具的`NPC`。

#### 创建数组

要使用 `Lua` 表格创建数组，只需按顺序存储各个值，并用逗号分隔这些值即可。数组值可以是任何非 `nil` 类型（布尔值、数字、字符串、函数、用户数据，甚至是另一个表格）。

```lua
-- 构建一个由三个项组成的数组
local tArray = {"A字符串", 1.2345, workspace.Object}
```

#### 从数组读取数据

要从数组中读取数据，请在其引用后添加一对方括号，并指定其中元素的索引号 `([pos])`：
```lua
-- 构建三个项组成的数组
local tArray = {"A字符串", 1.2345, workspace.Object}
 
print(tArray[1])
print(tArray[2])
print(tArray[3])
```

  >与某些语言不同，`Lua` 对数组使用以 `1` 为基数的索引，这意味着数组中的第一项是 `[1]`，而不是 `[0]`。

#### 向数组写入数据

可以通过在方括号 `([pos])` 中指示索引号，并后跟 `=` 和值来定义或重写数组索引值：

```lua
local tArray = {"A string", 1.2345, workspace.Object}
 
tArray[2] = 12345
tArray[4] = "B字符串"
 
print(tArray[2])
print(tArray[4])
```

#### 循环访问数组

  可以通过以下两种方式循环访问（循环遍历）数组：
   * 在 `for` 循环中使用内置的 `ipairs()` 函数。
   * 使用 `#` 运算符获取数组的长度，并从 `1` 一直循环到该长度值。

```lua
local tArray = {"A字符串", 1.2345, workspace.Object, "B字符串"}
 
-- 用“ipairs()”循环
for index, value in ipairs(tArray) do
	print(index, value)
end
 
-- 用数组长度运算符（#）迭代
for index = 1, #tArray do
	print(index, tArray[index])
end
```

#### 插入项目

  可以通过以下两种方法之一向数组末尾插入项目：
   * 将数组引用和项目值传递给 `Lua` 的 `table.insert()` 函数。
   * 使用 `t[#t+1]` 语法将新项目添加到数组。

```lua
local tArray = {"A字符串", 1.2345}
 
table.insert(tArray, "B字符串")
tArray[#tArray+1] = "C字符串"
 
print(tArray[3])
print(tArray[4])
```

  此外，也可以通过将位置值作为 `table.insert()` 的第二个参数，在开头和结尾之间插入项目。此方法将插入新项目，并将随后的项目上移一个索引位置。

```lua
local tArray = {"第一个项", "第二个项"}
 
table.insert(tArray, 2, "新项 #2")
 
print(tArray[1])
print(tArray[2])
print(tArray[3])
```

#### 移除项目

可以使用 `Lua` 的 `table.remove()` 函数从数组中移除项目。此方法将移除指定位置处的项目，并将随后的所有项目下移一个索引位置。

```lua
local tArray = {"第一个项", "第二个项", "最后一项"}
 
table.remove(tArray, 2)
 
print(tArray[1])
print(tArray[2])
```

------------------------------------------------------------------------------------------
## 字典

字典是对数组的扩展。数组存储一组有序的项目，而字典存储一组键值对。

|键|值|
|:---   |:---|
|BlockName   |GrassCube   |
|BlockColor|Green   |
|Place|true   |

#### 创建字典

要创建字典表，请定义每个键，并后跟 `=` 和值。请记得用逗号分隔每个键值对：

```lua
local tDictionary = {
	BlockName = "草块",
	BlockColor = "绿色",
	IsReplaceable = true
}
```

在创建字典时，键不仅限于字符串名称（如 `BlockColor`）；例如，键也可以是 `SandboxNode`。在这种情况下，必须用方括号 `([key])` 声明键：

```lua
local part = SandboxNode.New("Model")
 
local tDictionary = {
	PartType = "Block",
	[part] = true
}
```

#### 从字典中读取数据

要从字典中读取数据，请在其引用后添加一对方括号并指定键名称：

```lua
local part = SandboxNode.New("Model")
 
local tDictionary = {
	PartType = "Block",
	[part] = true
}
 
print(tDictionary["PartType"])  -- 字符串键带引号
print(tDictionary[part])  -- 非字符串键不带引号
```

  如上面的代码注释中所述，请注意以下几点：
  * 必须用引号将字符串键（例如 `PartType`）引起来，如 `tDictionary["PartType"]` 中的情况。
  * 不应使用引号将非字符串键（例如 `[part]`）引起来。

#### 向字典写入数据

可以通过在方括号 `([key])` 中指示键名称并后跟 `=` 和值来定义新的或现有的字典键的值：
```lua
local tDictionary = {
	BlockName = "草块",
	IsReplaceable = true
}
 
-- 变更现有键的值
tDictionary["BlockName"] = "沙块"
tDictionary["IsReplaceable"] = false
 
-- 插入新键值对
tDictionary["BlockCount"] = 10
 
print(tDictionary["BlockName"])
print(tDictionary["IsReplaceable"])
print(tDictionary["BlockCount"])
```

#### 循环访问字典

可以在 `for` 循环中使用内置的 `pairs()` 函数对字典进行循环访问：
```lua
local tDictionary = {
	BlockName = "草块",
	BlockColor = "绿色",
	IsReplaceable = true
}
 
for key, value in pairs(tDictionary) do
	print(key, value)
end
```
  >与对数组使用 `ipairs()` 不同，通过 `pairs()` 循环访问字典时不一定会按照项目在字典中的相同声明顺序返回这些项目。

#### 移除键值对

要从字典中移除键值对，只需将其值设置为 `nil` 即可，这会从字典中完全删除键值对，如下面的 `pairs()` 循环输出中所示：

```lua
local tDictionary = {
	BlockName = "草块",
	BlockColor = "绿色",
	IsReplaceable = true
}
 
tDictionary["IsReplaceable"] = nil
 
for key, value in pairs(tDictionary) do
	print(key, value)
end
```

------------------------------------------------------------------------------------------
## 将表作为引用

如果将表存储在新变量中，则不会创建该表的副本。该变量将成为原始表的引用（指针）。这意味着对原始表的任何更改都将反映在任何引用中：

```lua
local originalArray = {10, 20}
 
local arrayReference = originalArray
 
print("原数组：", originalArray[1], originalArray[2])
print("引用：", arrayReference[1], arrayReference[2])
 
-- 变更原数组中的值
originalArray[1] = 1000
originalArray[2] = 2000
 
print("引用：", arrayReference[1], arrayReference[2])
```