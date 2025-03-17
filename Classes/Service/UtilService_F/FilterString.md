# FilterString

*所属类*：
* [UtilService](/Api/Classes/Service/UtilService.md)
------------------------------------------------------------------------------------------
## 描述

过滤含有屏蔽字符的字符串

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|textTable|[Table](/Api/DataType/Table.md)||详见示例|

------------------------------------------------------------------------------------------
## 返回值

|<div style="width:150px">返回类型</div>|<div style="width:520px">概要</div>|
|:---|:---|
|[Bool](/Api/DataType/Bool.md)|IsBlocked:布尔值，true表示有屏蔽字符，false表示没有|
|[String](/Api/DataType/String.md)|text:字符串，这里返回经过屏蔽词处理后的字符串|

## **示例**

```lua
-- 节点脚本编辑
local util = game:GetService("UtilService")
--敏感词过滤 ，长度限制1024 
local result = util:FilterString({ text = "123456"})
--返回过滤后的文本
print( " text= ", result.text)
```

## 
