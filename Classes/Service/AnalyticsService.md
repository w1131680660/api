# AnalyticsService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ReportData</font>](/Api/Classes/Service/AnalyticsService_F/ReportData.md) ([ReflexMap](/Api/Enums/ReflexMap.md) dataMap)</div>|
|:---|
|数据埋点上报|

## 代码示例

```lua
-- 埋点立即上报
local function ReportSend(data)
	local  analyService = game:GetService("AnalyticsService")
	analyService:ReportData(data)
end

local reportData = {
	["scene_id"] = "1003",    --必要 场景ID
	["card_id"] = "OGM_GAME_MODE_1", --必要 栏目ID
	["comp_id"] = "MainPage", --必要 组件ID
	["event_code"] = "click", --必要 事件
	["standby1"] = "1",  --可选 需要上报的公参字段表
	["standby2"] = "2",
	["standby3"] = "3",
	["standby4"] = "4",
	["standby5"] = "5",
	["standby6"] = "6",
	["standby7"] = "7",
	["standby8"] = "8",
	["standby9"] = "9",
	["standby10"] = "10",
}
ReportSend(reportData)
```