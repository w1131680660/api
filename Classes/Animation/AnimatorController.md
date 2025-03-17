# AnimatorController

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的资源|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Classes/Animation/AnimatorController_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetStateMachineCount</font>](/Api/Classes/Animation/AnimatorController_F/GetStateMachineCount.md) ()</div>|
|:---|
|获取当前持有的状态机个数|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetStateMachine</font>](/Api/Classes/Animation/AnimatorController_F/GetStateMachine.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|通过下标获取当前持有的状态机数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetStateMachineByName</font>](/Api/Classes/Animation/AnimatorController_F/GetStateMachineByName.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|通过状态机名获取当前持有的状态机数据|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">CreateLayer</font>](/Api/Classes/Animation/AnimatorController_F/CreateLayer.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|新建一个AnimatorLayerData实例|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveLayer</font>](/Api/Classes/Animation/AnimatorController_F/RemoveLayer.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|通过layer名移除一个AnimatorLayerData实例|

