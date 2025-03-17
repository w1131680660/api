# SandboxNode

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">ClassType</font></div>|
|:---|
|节点的ClassType名称（不可写）|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Name</font></div>|
|:---|
|节点名|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Tag</font></div>|
|:---|
|节点标签|

|<div style="width:700px">[SandboxNode](/Api/Enums/SandboxNode.md) &emsp;<font color="dd00dd">Parent</font></div>|
|:---|
|父节点|

|<div style="width:700px">[SandboxNode](/Api/Enums/SandboxNode.md) &emsp;<font color="dd00dd">parent</font></div>|
|:---|
|父节点（仅脚本可调用）|

|<div style="width:700px">[SandboxNode](/Api/Enums/SandboxNode.md) &emsp;<font color="dd00dd">Children</font></div>|
|:---|
|全部子节点。（仅脚本可调用）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Enabled</font></div>|
|:---|
|节点是否被禁用。被禁用后节点内逻辑，事件，通知等不生效。|

|<div style="width:700px">[AttributeContainer](/Api/Enums/AttributeContainer.md) &emsp;<font color="dd00dd">Attibutes</font></div>|
|:---|
|获取属性容器。（仅脚本可调用）|

|<div style="width:700px">[NodeSyncMode](/Api/Enums/NodeSyncMode.md) &emsp;<font color="dd00dd">SyncMode</font></div>|
|:---|
|同步模式（仅主机能够设置）|

|<div style="width:700px">[NodeSyncLocalFlag](/Api/Enums/NodeSyncLocalFlag.md) &emsp;<font color="dd00dd">LocalSyncFlag</font></div>|
|:---|
|本地同步标识（本地属性，不需要同步）|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IgnoreSafeMode</font></div>|
|:---|
|忽略安全模式|

|<div style="width:700px">[ResourceLoadMode](/Api/Enums/ResourceLoadMode.md) &emsp;<font color="dd00dd">ResourceLoadMode</font></div>|
|:---|
||

|<div style="width:700px">[unsignedlonglong](/Api/Enums/unsignedlonglong.md) &emsp;<font color="dd00dd">FlagDebug</font></div>|
|:---|
||

|<div style="width:700px">[SandboxNodeID](/Api/Enums/SandboxNodeID.md) &emsp;<font color="dd00dd">ID</font></div>|
|:---|
|节点ID|

|<div style="width:700px">[SandboxNodeID](/Api/Enums/SandboxNodeID.md) &emsp;<font color="dd00dd">ID</font></div>|
|:---|
|节点ID|

## 成员函数

|<div style="width:700px">[SandboxNode](/Api/Enums/SandboxNode.md) &emsp;[<font color="dd00dd">Clone</font>](/Api/Classes/Base/SandboxNode_F/Clone.md) ()</div>|
|:---|
|节点克隆，克隆反射属性，自定义属性，以及包含的子对象|

|<div style="width:700px">[SandboxNode](/Api/Enums/SandboxNode.md) &emsp;[<font color="dd00dd">FindFirstChild</font>](/Api/Classes/Base/SandboxNode_F/FindFirstChild.md) ()</div>|
|:---|
|通过节点名找到节点对象|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Destroy</font> ()</div>|
|:---|
|销毁节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ClearAllChildren</font> ()</div>|
|:---|
|清除所有子节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetParent</font> ()</div>|
|:---|
|设置父节点|

|<div style="width:700px">[SandboxNodeID](/Api/Enums/SandboxNodeID.md) &emsp;[<font color="dd00dd">GetNodeid</font>](/Api/Classes/Base/SandboxNode_F/GetNodeid.md) ()</div>|
|:---|
|获取节点id|

|<div style="width:700px">[ReflexVariant](/Api/Enums/ReflexVariant.md) &emsp;[<font color="dd00dd">GetAttribute</font>](/Api/Classes/Base/SandboxNode_F/GetAttribute.md) ()</div>|
|:---|
|获取attr的反射属性|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetAttribute</font>](/Api/Classes/Base/SandboxNode_F/SetAttribute.md) ()</div>|
|:---|
|设置反射的属性值|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">AddAttribute</font> ()</div>|
|:---|
|添加一条反射属性|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">DeleteAttribute</font> ()</div>|
|:---|
|通过attr名删除一条反射属性|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsA</font>](/Api/Classes/Base/SandboxNode_F/IsA.md) ()</div>|
|:---|
|判断节点的ClassType是不是属于value代表的ClassType|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetReflexSyncMode</font> ()</div>|
|:---|
|设置反射同步模式（仅主机能够设置）|

|<div style="width:700px">[SYNCMODE](/Api/Enums/NodeSyncMode.md) &emsp;[<font color="dd00dd">GetReflexSyncMode</font>](/Api/Classes/Base/SandboxNode_F/GetReflexSyncMode.md) ()</div>|
|:---|
|获取反射同步模式|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetReflexLocalSyncFlag</font> ()</div>|
|:---|
|设置反射本地同步标记|

|<div style="width:700px">[SYNCLOCALFLAG](/Api/Enums/NodeSyncLocalFlag.md) &emsp;[<font color="dd00dd">GetReflexLocalSyncFlag</font>](/Api/Classes/Base/SandboxNode_F/GetReflexLocalSyncFlag.md) ()</div>|
|:---|
|获取反射本地同步标记|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ManualLoad</font> ()</div>|
|:---|
|同步|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ManualLoadAsync</font> ()</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ManualUnLoad</font> ()</div>|
|:---|
|主动卸载|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">AncestryChanged</font>](/Api/Classes/Base/SandboxNode_F/AncestryChanged.md) ([SandboxNode](/Api/Enums/SandboxNode.md) ancestry)</div>|
|:---|
|祖先节点变化时，会触发一个AncestryChanged通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">ParentChanged</font>](/Api/Classes/Base/SandboxNode_F/ParentChanged.md) ([SandboxNode](/Api/Enums/SandboxNode.md) parent)</div>|
|:---|
|父节点(或父级节点)变化时，会触发一个ParentChanged通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">AttributeChanged</font>](/Api/Classes/Base/SandboxNode_F/AttributeChanged.md) ([string](/Api/DataType/String.md) attr)</div>|
|:---|
|属性发生变化时，会触发一个AttributeChanged通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">ChildAdded</font>](/Api/Classes/Base/SandboxNode_F/ChildAdded.md) ([SandboxNode](/Api/Enums/SandboxNode.md) child)</div>|
|:---|
|新增子节点时，会触发一个ChildAdded通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">ChildRemoved</font>](/Api/Classes/Base/SandboxNode_F/ChildRemoved.md) ([SandboxNode](/Api/Enums/SandboxNode.md) child)</div>|
|:---|
|移除子节点时，会触发一个ChildRemoved通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">CustomAttrChanged</font>](/Api/Classes/Base/SandboxNode_F/CustomAttrChanged.md) ([string](/Api/DataType/String.md) attr)</div>|
|:---|
|自定义属性发生变化，会触发一个CustomAttrChanged通知|

## 代码示例

```lua
--SandboxNode node 有一个自定义属性 bool类型 名字是test_k
local v = node:GetAttribute("test_k")
```