# String

------------------------------------------------------------------------------------------
## 描述

`String`（字符串）可以用来代表一组字母、数字和符号，是脚本编写的重要组成部分。

------------------------------------------------------------------------------------------
#### 字符串的声明

声明字符串时最常用到的方法为在字符串的内容前后添加双引号`（"）`。下列声明将会使变量 `str` 中包含内容为 `Hello world!` 的字符串：

```lua
local str = "Hello world!"
```

同时，开发者也可以使用单引号 `（'）` 声明字符串。该方法在字符串本身包含双引号的情况下十分有用：

```lua
local str1 = 'Hello "World"!'
local str2 = "Hello "World"!"  -- This will cause an error
 
print(str1)
```

另外，我们也可以通过双括号`([[)`对字符串进行声明。此方法对于存储多行字符串的情况十分有用：

```lua
local str = [[This is a string that,
when printed, will appear
on multiple lines]]
 
print(str)
```

#### 字符串的合并

字符串可以通过名为 `Concatenation`（串联）的方法进行合并。`Lua` 语言中的串联语法是在字符串之间使用两个点 `（..）`。请参考以下示例：

```lua
local str = "Your high score is "
local highScore = 5200
 
local combinedString = str .. highScore
 
print(str)
print(combinedString)
```

  >注意：串联语法不会在两个字符串之间插入空格。当需要在两个被合并的字符串中间添加空格时，开发者需要在第一个字符串末尾（或第二个字符串开头）添加空格，如上面代码示例的第 `1` 行所示。

#### 字符串的转换

开发者可以通过 `tonumber()` 函数轻松将字符串转换为数字。此函数将会获取一个参数（字符串）并将其作为数字返回。如果字符串并非数字（例如 `"Hello"`），则 `tonumber()` 函数将会返回 `nil`。

```lua
local str1 = "123"
local str2 = "Hello"
 
print(tonumber(str1))
print(tonumber(str2))
```

同时，开发者也可以使用 `tostring()` 函数将数字转换为字符串。请参考以下示例：

```lua
local highScore = 5200
print(type(highScore))
 
local converted = tostring(highScore)
print(type(converted))
```


#### 字符串与数学运算

在使用字符串值进行数学运算时，`Lua` 会自动尝试将字符串转换为数字，因此开发者将无需事先将字符串封装在 `tonumber()` 中。当字符串无法被转换为数字时，脚本将会报错。

```lua
print("50" + 10)
```

```lua
print("Hello" + 10)
```

#### 字符串的转义

在双引号或单引号字符串声明（但不包括双括号声明）中，可以使用反斜线`（\）`嵌入几乎所有字符。以下是另一种在字符串中包含引号的有用方法：

```lua
local str = "Hello \"World\"!"
 
print(str)
```

  >请注意：在使用字符串转义符时，反斜线后面的某些字符具有特殊含义。举例来说，`\n` 将会生成换行符而不是转义字符 `n`。

```lua
-- \n = newline
local str = "Hello\nWorld!"
 
print(str)
```

```lua
-- \t = horizontal tab
local str = "Hello\tWorld!"
 
print(str)
```