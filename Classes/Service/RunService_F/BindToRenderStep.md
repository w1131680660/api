# BindToRenderStep

*所属类*：
* [RunService](/Api/Classes/Service/RunService.md)
------------------------------------------------------------------------------------------
## 描述

绑定RenderStep事件的Lua函数。RenderPriority为当前游戏内渲染层级，可根据需要进行插入

------------------------------------------------------------------------------------------
## 参数

|<div style="width:100px">名称</div>|<div style="width:100px">类型</div>|<div style="width:50px">默认</div>|<div style="width:350px">描述</div>|
|:---|:---|:---|:---|
|szKey|[string](/Api/DataType/String.md)||绑定标记key|
|priority|[int](/Api/DataType/Number.md)||渲染层级|
|func|[LuaFunction](/Api/DataType/LuaFunction.md)||Lua函数|
