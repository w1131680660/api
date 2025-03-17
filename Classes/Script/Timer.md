# Timer

## 属性

|<div style="width:700px">[LuaFunction](/Api/Enums/LuaFunction.md) &emsp;<font color="dd00dd">Callback</font></div>|
|:---|
|lua回调方法|

|<div style="width:700px">[double](/Api/Enums/double.md) &emsp;<font color="dd00dd">Delay</font></div>|
|:---|
|首次延迟执行的时间|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Loop</font></div>|
|:---|
|是否循环执行|

|<div style="width:700px">[double](/Api/Enums/double.md) &emsp;<font color="dd00dd">Interval</font></div>|
|:---|
|计时间隔时间|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Start</font> ()</div>|
|:---|
|开始执行|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Pause</font> ()</div>|
|:---|
|暂停。需要在开始执行后调用|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Resume</font> ()</div>|
|:---|
|恢复。需要在暂停后调用|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Stop</font> ()</div>|
|:---|
|停止。需要在开始执行后调用|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">StartEx</font>](/Api/Classes/Script/Timer_F/StartEx.md) ([double](/Api/Enums/double.md) delay, [bool](/Api/DataType/Bool.md) loop, [double](/Api/Enums/double.md) interval, [LuaFunction](/Api/Enums/LuaFunction.md) cb)</div>|
|:---|
|开始执行。附带初始化的参数此服务器中可以容纳的最大玩家数量|

|<div style="width:700px">[RUNSTATE](/Api/Enums/TimerRunState.md) &emsp;[<font color="dd00dd">GetRunState</font>](/Api/Classes/Script/Timer_F/GetRunState.md) ()</div>|
|:---|
|获取定时器运行状态|

## 代码示例

```lua
local a = 0
local timer = SandboxNode.new("Timer") -- 创建定时器节点
timer.Delay = 1 -- 延迟多少秒开始
timer.Loop = true -- 是否循环
timer.Interval = 2 -- 循环间隔多少秒
timer.Callback = function() -- 回调方法
	a = a + 1
	print("timer : ", timer, " a=", a)
	if a == 4 then
		print("timer pause")
		timer:Pause() -- 暂停定时器，只有在定时器运行期间有效
		wait(4)
		print("timer resume")
		timer:Resume() -- 恢复定时器，只有在定时器运行暂停期间有效
	end
end
timer:Start()

-- 一次性传入参数，并且开始定时器
--timer:StartEx(3, true, 3, function() a = a + 1; print("timer ex : a=", a) end)
print("timer start")
```