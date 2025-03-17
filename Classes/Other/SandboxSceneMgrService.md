# SandboxSceneMgrService

## 属性

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;<font color="dd00dd">SceneConfigs</font></div>|
|:---|
||

|<div style="width:700px">[EMultiScenes](/Api/Enums/EMultiScenes.md) &emsp;<font color="dd00dd">CurDefaultStartScene</font></div>|
|:---|
|动态场景配置|

|<div style="width:700px">[EMultiScenes](/Api/Enums/EMultiScenes.md) &emsp;<font color="dd00dd">NextDefaultStartScene</font></div>|
|:---|
||

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;<font color="dd00dd">DynamicSceneConfigs</font></div>|
|:---|
||

## 函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SwitchScene</font> ()</div>|
|:---|
|切换场景(客户端)切换结果SceneOpResult通知回调|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">AddDynamicScene</font> ()</div>|
|:---|
|添加动态场景(服务端)添加结果DynamicSceneOpResultServer通知回调|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">RemoveDynamicScene</font> ()</div>|
|:---|
|删除动态场景(服务端)删除结果DynamicSceneOpResultServer通知回调|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">DynamicSwitchScene</font> ()</div>|
|:---|
|切换结果DynamicSceneOpResultServer通知回调|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">SceneSwitchStart</font> ()</div>|
|:---|
|切换场景开始通知(客户端)|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">SceneOpResult</font>](/Api/Classes/Other/SandboxSceneMgrService_F/SceneOpResult.md) ([unsignedchar](/Api/DataType/unsignedchar.md) type, [unsignedshort](/Api/DataType/unsignedshort.md) sceneid, [int](/Api/DataType/Number.md) result)</div>|
|:---|
|场景操作结果通知(客户端)|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">DynamicSceneOpResultServer</font>](/Api/Classes/Other/SandboxSceneMgrService_F/DynamicSceneOpResultServer.md) ([unsignedchar](/Api/DataType/unsignedchar.md) type, [unsignedshort](/Api/DataType/unsignedshort.md) sceneid, [int](/Api/DataType/Number.md) result, [int](/Api/DataType/Number.md) uid)</div>|
|:---|
|动态场景操作结果通知(服务端)|

