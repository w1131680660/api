# BindContext

*所属类*:
* [ContextActionService](/Api/Classes/Input/ContextActionService.md)
------------------------------------------------------------------------------------------
## 描述

绑定一个回调函数到指定输入上

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|actionname|[string](/Api/DataType/String.md)||自定义的名称，代表本次绑定|
|func|[LuaFunction](/Api/Enums/LuaFunction.md)||lua回调函数（三个参数1.actionName类型：string描述：最初传递给BindAction的相同字符串;2.state类型：int描述：当前事件的输入状态，等于UserInputState中的值;3.inputObj类型：携带输入信息的对象）|
|createTouchBtn|[bool](/Api/DataType/Bool.md)||是否创建触摸按钮|
|hotkey|[ReflexVariant](/Api/Enums/ReflexVariant.md)||快捷键|
