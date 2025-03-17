# CoreUI

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HideBtnExit</font></div>|
|:---|
|是否隐藏退出按钮|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HideBtnMsg</font></div>|
|:---|
|是否隐藏消息按钮|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HideViewRoomInfo</font></div>|
|:---|
|是否隐藏房间信息视图|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">MicUnMute</font></div>|
|:---|
|麦克风是否静音|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HornUnMute</font></div>|
|:---|
|喇叭是否静音|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">HideBtnSet</font></div>|
|:---|
|是否隐藏设置按钮|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ExitGame</font> ()</div>|
|:---|
|退出游戏|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">MicSwitchBtn</font> ()</div>|
|:---|
|麦克风开关按钮|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">HornSwitchBtn</font> ()</div>|
|:---|
|喇叭开关按钮|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetHeadNode</font>](/Api/Classes/Scene/CoreUI_F/GetHeadNode.md) ([string](/Api/DataType/String.md) uin)</div>|
|:---|
|获取用户头像|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">CheckEnv</font>](/Api/Classes/Scene/CoreUI_F/CheckEnv.md) ([bool](/Api/DataType/Bool.md) bCheck)</div>|
|:---|
|检查环境|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetRandomNickName</font>](/Api/Classes/Scene/CoreUI_F/GetRandomNickName.md) ([int](/Api/DataType/Number.md) nSex)</div>|
|:---|
|获取随机昵称|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetRandomAvatar</font>](/Api/Classes/Scene/CoreUI_F/GetRandomAvatar.md) ()</div>|
|:---|
|获取随机头像|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">CheckCoreUiHide</font>](/Api/Classes/Scene/CoreUI_F/CheckCoreUiHide.md) ([EnumCoreUi](/Api/Enums/CoreUiComponent.md) val)</div>|
|:---|
|检测ui是否被隐藏|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">HideCoreUi</font>](/Api/Classes/Scene/CoreUI_F/HideCoreUi.md) ([EnumCoreUi](/Api/Enums/CoreUiComponent.md) val)</div>|
|:---|
|屏蔽CoreUi默认组件|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">OpenWareHouse</font> ()</div>|
|:---|
|打开玩家仓库皮肤界面|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetSnapshot</font>](/Api/Classes/Scene/CoreUI_F/GetSnapshot.md) ([int](/Api/DataType/Number.md) val)</div>|
|:---|
|获取截屏|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">DoSnapshot</font>](/Api/Classes/Scene/CoreUI_F/DoSnapshot.md) ([int](/Api/DataType/Number.md) )</div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;<font color="dd00dd">UiChange</font> ()</div>|
|:---|
|UI发生变化时，会触发一个UiChange通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">SnapshotFinish</font>](/Api/Classes/Scene/CoreUI_F/SnapshotFinish.md) ([bool](/Api/DataType/Bool.md) , [Texture2D>](/Api/Enums/Texture2D>.md) )</div>|
|:---|
||

