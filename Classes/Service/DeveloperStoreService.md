# DeveloperStoreService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GetDeveloperStoreItems</font> ()</div>|
|:---|
|查询当前地图开发者商店列表|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GetPlayerDeveloperProducts</font> ()</div>|
|:---|
|查询指定玩家的购买商品信息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ServiceGetPlayerDeveloperProducts</font> ()</div>|
|:---|
|云服查询指定玩家的购买商品信息|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">GetProductInfo</font>](/Api/Classes/Service/DeveloperStoreService_F/GetProductInfo.md) ([int](/Api/DataType/Number.md) productid)</div>|
|:---|
|查询指定商品(开发者商店中商品)的信息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BuyGoods</font>](/Api/Classes/Service/DeveloperStoreService_F/BuyGoods.md) ([int](/Api/DataType/Number.md) goodsid, [string](/Api/DataType/String.md) goodsdesc, [int](/Api/DataType/Number.md) goodsnum)</div>|
|:---|
|弹出购买弹窗|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">BuyGoods</font>](/Api/Classes/Service/DeveloperStoreService_F/BuyGoods.md) ([int](/Api/DataType/Number.md) goodsid, [string](/Api/DataType/String.md) goodsdesc, [int](/Api/DataType/Number.md) goodsnum, [string](/Api/DataType/String.md) extraDesc)</div>|
|:---|
|弹出购买弹窗|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">MiniCoinRecharge</font> ()</div>|
|:---|
|打开Mini币充值弹窗|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GetPlayerDeveloperSingleProducts</font> ()</div>|
|:---|
|查询指定玩家的购买单个商品信息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ServiceGetPlayerDeveloperSingleProducts</font> ()</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GetAllStoreItems</font> ()</div>|
|:---|
|查询所有仓库内商品|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GetStoreItemsByID</font> ()</div>|
|:---|
|按ID查询仓库内商品的数量|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">DeleteStoreItems</font> ()</div>|
|:---|
|删除仓库ID位置的物品|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">AddStoreItemsArguments</font> ()</div>|
|:---|
|备注字段，给仓库id位置的物品添加一段参数。|

## 代码示例

```lua

--客户端脚本LocalScript

local store = game:GetService("DeveloperStoreService")

-- 获取地图开发者商店商品列表
local function GetStoreList()
	local storeList = store:GetDeveloperStoreItems()
	print("store list = ", storeList)
	local listLength = #storeList
	if listLength > 0 then
		-- 遍历每个商品信息
		local storeitem = {}
		for _, value in pairs(storeList) do
			print("store list key = ", _)
			for key, info in pairs(value) do
				storeitem[key] = info
				print("store list key = ", key)
				print("store list info = ", info)
			end
		end
	end
	return storeList
end

-- 获取玩家已购买的商品列表
local function GetPurchasedList()
	local buyList = store:GetPlayerDeveloperProducts()
	print("store buy list = ", buyList)
	local buyListLength = #buyList
	if buyListLength > 0 then
		-- 遍历每个商品信息
		local buyItem = {}
		for _, value in pairs(buyList) do
			print("store buy list key = ", _)
			for key, info in pairs(value) do
				buyItem[key] = info
				print("store buy list key = ", key)
				print("store buy list info = ", info)
			end
		end
	end
	return buyList
end

-- 获取地图开发者商店某个商品详细信息
local function GetGoodsInfo(goodsid)
	local goodsInfo = store:GetProductInfo(goodsid)
	if goodsInfo.name ~= nil then
		print("goods name = ", goodsInfo["name"])
	end
	if goodsInfo.desc ~= nil then
		print("goods desc = ", goodsInfo["desc"])
	end
	if goodsInfo.goodId ~= nil then
		print("goods goodId = ", goodsInfo["goodId"])
	end
	if goodsInfo.costType ~= nil then
		print("goods costType = ", goodsInfo["costType"])
	end
	if goodsInfo.costNum ~= nil then
		print("goods costNum = ", goodsInfo["costNum"])
	end
	if goodsInfo.download ~= nil then
		print("goods download = ", goodsInfo["download"])
	end
	if goodsInfo.cover ~= nil then
		print("goods cover = ", goodsInfo["cover"])
	end
	return goodsInfo
end

-- 购买开发者商店某个商品
local function BuyGoods(goodsid, num)
	local info = GetGoodsInfo(goodsid)
	if info ~= nil and info.desc ~= nil then
		local goodDesc = info["desc"]
		store:BuyGoods(goodsid, goodDesc,num)
	end
end

-- 充值弹窗
local function CoinRecharge()
	store:MiniCoinRecharge()
end

GetStoreList()  -- 获取开发者商店列表
GetPurchasedList()  -- 客户端获取已购买商品列表

wait(10)
local goodsid = 530001   -- 530001 ~ 539999
BuyGoods(goodsid，1)

CoinRecharge()  --主动充值


-- 服务端脚本 Script

local store = game:GetService("DeveloperStoreService")
store.RemoteBuyGoodsCallBack:Connect(function(uin, goodsid, code, msg, num)
	if code ~= 0 then
		print("Goods purchase failed.")
		print("Error code: ",code)
		print("Error message : ",msg)
		--0-购买成功
		--1001-地图未上传
		--1002-用户取消购买
		--1003-此商品查询失败
		--1004-请求失败
		--1005-迷你币不足
		--
		--710-商品不存在
		--711-商品状态异常
		--712-不能购买自己的商品
		--713-已购买该商品，不能重复购买
		--714-购买失败，购买数量已达上限
		--
		return
	end
	--code=0 购买成功
	print("Goods purchase Success.")
	print("RemoteBuyGoodsCallBack - uin : ",uin)
	print("RemoteBuyGoodsCallBack - goodsid: ",goodsid)
	print("RemoteBuyGoodsCallBack - num: ",num)
	print("Do something") --装备道具
end)

-- 服务器：获取某个玩家已购买的商品列表
local function GetPlayerPurchasedList(playerid)
	local buyList = store:ServiceGetPlayerDeveloperProducts(playerid)
	print("cloud store buy list = ", buyList)
	local buyListLength = #buyList
	if buyListLength > 0 then
		-- 遍历每个商品信息
		local buyItem = {}
		for _, value in pairs(buyList) do
			print("cloud buy list key = ", _)
			for key, info in pairs(value) do
				buyItem[key] = info
				print("cloud buy list key = ", key)
				print("cloud buy list info = ", info)
			end
		end
	end
	return buyList
end

```