# Environment

## 属性

|<div style="width:700px">[EnumWeather](/Api/Enums/EnumWeather.md) &emsp;<font color="dd00dd">Weather</font></div>|
|:---|
|设置天气类型:晴天、雨天、打雷和自定义|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Gravity</font></div>|
|:---|
|环境重力效果设置|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TimeHour</font></div>|
|:---|
|时间设置|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">LockTimeHour</font></div>|
|:---|
|是否锁定时间|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TimeHour</font></div>|
|:---|
|时间设置|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">LockTime</font>](/Api/Classes/Build/Environment_F/LockTime.md) ([float](/Api/DataType/Number.md) timehour)</div>|
|:---|
|锁定时间（兼容旧版，应该废弃）|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">WeatherChanged</font>](/Api/Classes/Build/Environment_F/WeatherChanged.md) ([int](/Api/DataType/Number.md) weather)</div>|
|:---|
|当天气改变时，会触发一个WeatherChanged通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">GravityChanged</font>](/Api/Classes/Build/Environment_F/GravityChanged.md) ([float](/Api/DataType/Number.md) gravity)</div>|
|:---|
|当重力改变时，会触发一个GravityChanged通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">TimeChanged</font>](/Api/Classes/Build/Environment_F/TimeChanged.md) ([float](/Api/DataType/Number.md) timehour)</div>|
|:---|
|当时间改变时，会触发一个TimeChanged通知|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local environment = workspace.Environment
--设置天气为下雨
environment.Weather = Enum.Weather.Rain
--设置天空为火山
environment.SkyPlanet = Enum.SkyPlanet.Volcano
--设置时间为22
environment.TimeHour = 22
```