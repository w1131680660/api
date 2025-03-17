# SandboxUISnapshotNode

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsSnapFinish</font></div>|
|:---|
|是否截屏完毕|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">OnSnapFinish</font> ()</div>|
|:---|
|截屏完毕时，触发一个OnSnapFinish通知|

## 代码示例

```lua
	CoreUI = game:GetService("CoreUI")

	if not CoreUI then
		return
	end

	function Snapshot()
		local SnapshotNode = CoreUI:GetSnapshot(1)

		print(SnapshotNode)

		if not SnapshotNode then
		  print("call 'CoreUI:GetSnapshot' return nil")
		  return
		end

		local  PlayerGui = game:GetService("Players").LocalPlayer.PlayerGui
		local TouchUIMain = PlayerGui.TouchUIMain

		SnapshotNode.Parent = TouchUIMain
		SnapshotNode.Size = Vector2.new(400, 300)
		SnapshotNode.Position = Vector2.new(400, 300)

		SnapshotNode.OnSnapFinish:connect(function()
			SnapshotNode.BlurFilter = true
			SnapshotNode.BlurSigma = 2
		end)
	end
	//按j截屏
	local contextActionService = game:GetService("ContextActionService")
	contextActionService:BindAction("Snapshot", Snapshot, Enum.ContextActionType.KeyBoard.Value, string.byte('j'))
```