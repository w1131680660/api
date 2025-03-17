# AdvertisementService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">PlayAdvertising</font>](/Api/Classes/Service/AdvertisementService_F/PlayAdvertising.md) ([int](/Api/DataType/Number.md) uin, [bool](/Api/DataType/Bool.md) success)</div>|
|:---|
|指定用户播放广告|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">PlayAdvertisingCallback</font>](/Api/Classes/Service/AdvertisementService_F/PlayAdvertisingCallback.md) ([LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|广告播放接口回调|

## 代码示例

```lua

  --目前只支持手机端播放广告
local advertService = game:GetService("AdvertisementService")

-- 播放广告
-- playerUin 指定哪个用户播放
local function PlayAdvertisements(playerUin, isSuccess)
	print('Advertisements start play!')
	adservice:PlayAdvertising(playerUin, isSuccess)
end

local function PlayFinished()
	local function LuaCallBack(msg)
		print("call back msg = ",msg)
		print('Advertisements play finished!')
	end
	adservice:PlayAdvertisingCallback(LuaCallBack)
end

--使用时优先注册广告播放完的回调
PlayFinished()

button.Click:Connect(function()
	-- 点击开始播放广告
	PlayAdvertisements(1000091378, true)
end)

```