# AnimatorStateMachineData

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的资源|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSubMachines</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/GetSubMachines.md) ()</div>|
|:---|
|获取当前持有的子状态机数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSubStateMachine</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/GetSubStateMachine.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|获取当前持有的一个子状态机数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetStates</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/GetStates.md) ()</div>|
|:---|
|获取当前持有的所有状态数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">CreateState</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/CreateState.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|创建一个状态数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetState</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/GetState.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|获取一个状态数据|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsEnter</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/IsEnter.md) ()</div>|
|:---|
|检查是否进入状态|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetFullName</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/GetFullName.md) ()</div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">EventNotify</font>](/Api/Classes/Animation/AnimatorStateMachineData_F/EventNotify.md) ([StateMachineMessage](/Api/Enums/StateMachineMessage.md) state)</div>|
|:---|
|发送一个当前状态机消息的通知|

