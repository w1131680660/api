# CollectionService

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">AddTag</font>](/Api/Classes/Service/CollectionService_F/AddTag.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [string](/Api/DataType/String.md) tag)</div>|
|:---|
|新增节点标签|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveTag</font>](/Api/Classes/Service/CollectionService_F/RemoveTag.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [string](/Api/DataType/String.md) tag)</div>|
|:---|
|移除节点标签|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetTagged</font>](/Api/Classes/Service/CollectionService_F/GetTagged.md) ([string](/Api/DataType/String.md) tag)</div>|
|:---|
|获取该标签的所有节点|

|<div style="width:700px">[table](/Api/DataType/Table.md) &emsp;[<font color="dd00dd">GetTags</font>](/Api/Classes/Service/CollectionService_F/GetTags.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|获取该节点的所有标签|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">HasTag</font>](/Api/Classes/Service/CollectionService_F/HasTag.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [string](/Api/DataType/String.md) tag)</div>|
|:---|
|该节点是否有标签|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">GetNodeAddedSignal</font>](/Api/Classes/Service/CollectionService_F/GetNodeAddedSignal.md) ([string](/Api/DataType/String.md) tag)</div>|
|:---|
|获取该标签新增的沙盒信号|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">GetNodeRemovedSignal</font>](/Api/Classes/Service/CollectionService_F/GetNodeRemovedSignal.md) ([string](/Api/DataType/String.md) tag)</div>|
|:---|
|获取该标签移除的沙盒信号|

