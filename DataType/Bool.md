# Bool

------------------------------------------------------------------------------------------
## 描述

`Boolean`（布尔值）是一种非常简单的数据类型，其值为 `true` 或 `false`。布尔值常用于例如下列代码的条件语句中：

```lua
local testBoolean = true
 
if testBoolean == true then
	-- Value of 'testBoolean' is true, so this condition is executed
else
	-- If value of 'testBoolean' is false, this condition is executed
end
```

------------------------------------------------------------------------------------------
## Lua 估算

在 `Lua` 中，如果某个值不是 `false` 或 `nil`，则在条件语句中使用时会将其视为 `“true”`。下面的代码仅输出 `Lua` 解释为 `true` 的值：

```lua
-- These values are all "true"
if true then
	print("true")
end
if 1 then
	print("1")
end
if "text" then
	print('"text"')
end
if {1, 2, 3} then
	print("{1, 2, 3}")
end
if workspace then
	print("workspace")
end
if "" then
	print('""')
end
 
-- But these values are not...
if false then
	print("false")
end
if nil then
	print("nil")
end
```

------------------------------------------------------------------------------------------
## 运算符

根据上述估算规则，带有 `Lua operators` （运算符）的条件语句工作方式如下所示：

#### And

如果为 `false` 或 `nil`，**and** 运算符返回第一个参数，否则返回第二个参数。

```lua
print(4 and 5)
print(nil and 12)
print(false and 12)
print(true and true)
print(true and false)
print(false and true)
print(false and false)
```

#### Or

**or** 运算符对两个值进行运算。如果第一个值 既不是 `false` 也不是 `nil`，则 **or** 运算符返回第一个值。如果第一个值是 `false` 或 `nil`，则该运算符返回第二个值。例如：

```lua
local y = x or 1
print(y)
```
  >之所以输出 `1`，是因为 `x` 不存在，因此为 `nil`。实际上，**or** 运算符是让我们选择 `1` 而不是 `nil`。

```lua
local x = false
local y = x or 1
print(y)
```
  >之所以也输出 `1`，是因为尽管 `x` 存在，但其值为 `false`。如果 `x` 为 `true`，则 **or** 运算符将选择 `x` 而不是 `1`。

#### Not

如果参数为 `false` 或 `nil`，则 **not** 运算符返回 `true`，否则返回 `false`。

```lua
print(not true)
print(not false)
print(not nil)
print(not "text")
print(not 0)
```