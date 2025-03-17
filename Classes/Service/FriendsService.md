# FriendsService

## 成员函数

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetSize</font>](/Api/Classes/Service/FriendsService_F/GetSize.md) ()</div>|
|:---|
|获取好友数量|

|<div style="width:700px">[ReflexTuple](/Api/Enums/ReflexTuple.md) &emsp;[<font color="dd00dd">GetFriendsInfoByIndex</font>](/Api/Classes/Service/FriendsService_F/GetFriendsInfoByIndex.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|根据好友的序列号拿到好友信息|

## 代码示例

```lua
------ 判断某人是否是好友 ----------
local function checkFriends(playerUin)
	local friendsService = game:GetService("FriendsService")
	local friendsNum = friendsService:GetSize() --获取好友数（总序列号）
	for i = 0,friendsNum-1,1 do --初值,终值，步数
		local uin,nickName,onLine = friendsService:GetFriendsInfoByIndex(i) --遍历好友
		local isFriend = false
		if playerUin == uin then --比对该uin和拉去的好友列表
			isFriend = true
		end
		if isFriend then
			print("%s: is friend",nickName)
		else
			print("%s: is not friend",nickName)
		end
	end
end
local playerUin = 1111  --已知某人的uin信息
checkFriends(playerUin)
```