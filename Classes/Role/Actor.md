# Actor

## 属性

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Movespeed</font></div>|
|:---|
|生物的移动速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">MaxHealth</font></div>|
|:---|
|生物的最大血量|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Health</font></div>|
|:---|
|生物的当前血量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoRotate</font></div>|
|:---|
|自动旋转|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">NoPath</font></div>|
|:---|
|actor是否具有寻路路径|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Gravity</font></div>|
|:---|
|actor受到的重力|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StepOffset</font></div>|
|:---|
|玩家可以攀越的高度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanAutoJump</font></div>|
|:---|
|可以自由跳跃|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SkinId</font></div>|
|:---|
|通过玩家控制的角色获取玩家迷你皮肤id|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SlopeLimit</font></div>|
|:---|
|玩家可行走的坡度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">JumpBaseSpeed</font></div>|
|:---|
|玩家跳跃起始速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">JumpContinueSpeed</font></div>|
|:---|
|持续按住跳跃键减缓降落速度使用|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">RunSpeedFactor</font></div>|
|:---|
|给Movespeed加倍|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">RunState</font></div>|
|:---|
|是否为跑步状态|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanPushOthers</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">MoveDirection</font></div>|
|:---|
|移动的方向|

|<div style="width:700px">[PhysicsRoleType](/Api/Enums/PhysicsRoleType.md) &emsp;<font color="dd00dd">PhysXRoleType</font></div>|
|:---|
|物理类型|

|<div style="width:700px">[StandardSkeleton](/Api/Enums/StandardSkeleton.md) &emsp;<font color="dd00dd">StandardSkeleton</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMoveEndTime</font>](/Api/Classes/Role/Actor_F/SetMoveEndTime.md) ([float](/Api/DataType/Number.md) endtime)</div>|
|:---|
|设定移动结束时间|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">MoveTo</font>](/Api/Classes/Role/Actor_F/MoveTo.md) ([Vector3](/Api/DataType/Vector3.md) target)</div>|
|:---|
|actor朝某个位置进行移动|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">MoveStep</font>](/Api/Classes/Role/Actor_F/MoveStep.md) ([Vector3](/Api/DataType/Vector3.md) vec)</div>|
|:---|
|actor移动vec向量的位移|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Move</font>](/Api/Classes/Role/Actor_F/Move.md) ([Vector3](/Api/DataType/Vector3.md) dir, [bool](/Api/DataType/Bool.md) relativeToCamera)</div>|
|:---|
|actor朝指定方向进行移动|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">StopMove</font> ()</div>|
|:---|
|停止调用Move或MoveTo接口的运行|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Jump</font>](/Api/Classes/Role/Actor_F/Jump.md) ([bool](/Api/DataType/Bool.md) jump)</div>|
|:---|
|actor跳跃函数，将参数设置为true时，actor将会跳跃|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetJumpInfo</font>](/Api/Classes/Role/Actor_F/SetJumpInfo.md) ([float](/Api/DataType/Number.md) baseSpeed, [float](/Api/DataType/Number.md) continueSpeed)</div>|
|:---|
|跳跃设置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">NavigateTo</font>](/Api/Classes/Role/Actor_F/NavigateTo.md) ([Vector3](/Api/DataType/Vector3.md) target)</div>|
|:---|
|自动寻路至指定位置，会自动寻找最佳路径移动至指定点,本函数立即返回|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">JumpCDTime</font>](/Api/Classes/Role/Actor_F/JumpCDTime.md) ([float](/Api/DataType/Number.md) time)</div>|
|:---|
|跳跃间隔，处于跳跃间隔内时无法跳跃|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetEnableContinueJump</font>](/Api/Classes/Role/Actor_F/SetEnableContinueJump.md) ([bool](/Api/DataType/Bool.md) enable)</div>|
|:---|
|设置是否能够连续跳跃|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">StopNavigate</font> ()</div>|
|:---|
|停止自动寻路|

|<div style="width:700px">[BehaviorState](/Api/Enums/BehaviorState.md) &emsp;[<font color="dd00dd">GetCurMoveState</font>](/Api/Classes/Role/Actor_F/GetCurMoveState.md) ()</div>|
|:---|
|获取当前行为状态。见枚举BehaviorState|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">FindNearestPolygonCenter</font>](/Api/Classes/Role/Actor_F/FindNearestPolygonCenter.md) ()</div>|
|:---|
|同步找到一个可以寻路过去的点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UseDefaultAnimation</font>](/Api/Classes/Role/Actor_F/UseDefaultAnimation.md) ([bool](/Api/DataType/Bool.md) use)</div>|
|:---|
|是否使用默认动作|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">BindCustomPlayerSkin</font> ()</div>|
|:---|
|自定义绑定玩家皮肤给actor|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Walking</font>](/Api/Classes/Role/Actor_F/Walking.md) ([bool](/Api/DataType/Bool.md) isWalking)</div>|
|:---|
|当开始行走时会发送一次事件，停止行走时会发送一次通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Standing</font>](/Api/Classes/Role/Actor_F/Standing.md) ([bool](/Api/DataType/Bool.md) isStanding)</div>|
|:---|
|结束站立时会发送一次事件，开始站立时会发送一次通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Jumping</font>](/Api/Classes/Role/Actor_F/Jumping.md) ([bool](/Api/DataType/Bool.md) isJumping)</div>|
|:---|
|跳跃开始时会发送一次事件，跳跃结束时会发送一次通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Flying</font>](/Api/Classes/Role/Actor_F/Flying.md) ([bool](/Api/DataType/Bool.md) isFlying)</div>|
|:---|
|飞行开始时会发送一次事件，飞行结束时会发送一次通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">Died</font>](/Api/Classes/Role/Actor_F/Died.md) ([bool](/Api/DataType/Bool.md) isDied)</div>|
|:---|
|死亡开始时会发送一次事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MoveStateChange</font>](/Api/Classes/Role/Actor_F/MoveStateChange.md) ([BehaviorState](/Api/Enums/BehaviorState.md) beforeState, [BehaviorState](/Api/Enums/BehaviorState.md) afterState)</div>|
|:---|
|当actor移动状态发送变化时会发送一次事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NavigateFinished</font>](/Api/Classes/Role/Actor_F/NavigateFinished.md) ([bool](/Api/DataType/Bool.md) isFinished)</div>|
|:---|
|自动寻路结束后发送事件|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">MoveFinished</font>](/Api/Classes/Role/Actor_F/MoveFinished.md) ([bool](/Api/DataType/Bool.md) isMoveFinished)</div>|
|:---|
|移动MoveTo结束后触发|

## 代码示例

```lua
--创建实例
local newActor = SandboxNode.New('Actor')
--设置名字
newActor.Name = "my_actor"
--设置模型
newActor.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100010")
--设置位置
newActor.Position = Vector3.New(500,700,500)
--设置父节点
newActor:SetParent(Workspace)
--设置速度
newActor.Movespeed = 2 
--监听MoveFineshed事件
newActor.MoveFinished:Connect(function(isMoveFinished)
        print("actor move:"..tostring(isMoveFinished))
end)

newActor.Walking:Connect(function()
        print("actor walking..")
end)
```