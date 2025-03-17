# Chat

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DefaultChat</font></div>|
|:---|
|是否加载默认聊天|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsUserChatEnable</font>](/Api/Classes/GamePlay/Chat_F/IsUserChatEnable.md) ([int](/Api/DataType/Number.md) userid)</div>|
|:---|
|是否允许聊天|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SendChatText</font>](/Api/Classes/GamePlay/Chat_F/SendChatText.md) ([string](/Api/DataType/String.md) text, [int](/Api/DataType/Number.md) type, [int](/Api/DataType/Number.md) targetuin, [int](/Api/DataType/Number.md) language)</div>|
|:---|
|发送文本消息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SendSystemMsg</font>](/Api/Classes/GamePlay/Chat_F/SendSystemMsg.md) ([string](/Api/DataType/String.md) text, [int](/Api/DataType/Number.md) targetuin)</div>|
|:---|
|发送系统消息|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SendChat</font>](/Api/Classes/GamePlay/Chat_F/SendChat.md) ([string](/Api/DataType/String.md) text, [int](/Api/DataType/Number.md) targetuin)</div>|
|:---|
|发送文本消息|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetFilterString</font>](/Api/Classes/GamePlay/Chat_F/GetFilterString.md) ([string](/Api/DataType/String.md) text)</div>|
|:---|
|过滤文本|

|<div style="width:700px">[longlong](/Api/Enums/longlong.md) &emsp;[<font color="dd00dd">ShowChatBubble</font>](/Api/Classes/GamePlay/Chat_F/ShowChatBubble.md) ([string](/Api/DataType/String.md) text, [bool](/Api/DataType/Bool.md) isShow, [int](/Api/DataType/Number.md) bubble, [Vector3](/Api/DataType/Vector3.md) position, [longlong](/Api/Enums/longlong.md) chatBubbleId)</div>|
|:---|
|显示聊天气泡|

|<div style="width:700px">[longlong](/Api/Enums/longlong.md) &emsp;[<font color="dd00dd">ShowEditorChatBubble</font>](/Api/Classes/GamePlay/Chat_F/ShowEditorChatBubble.md) ([string](/Api/DataType/String.md) text, [int](/Api/DataType/Number.md) bgIndex, [string](/Api/DataType/String.md) bgPath, [Vector3](/Api/DataType/Vector3.md) position)</div>|
|:---|
|显示工具端聊天气泡|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">UpdateEditorChatBubblePosition</font>](/Api/Classes/GamePlay/Chat_F/UpdateEditorChatBubblePosition.md) ([longlong](/Api/Enums/longlong.md) chatBubbleId, [Vector3](/Api/DataType/Vector3.md) position)</div>|
|:---|
|更新工具端聊天气泡位置|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetActorShowEditorChatBubble</font>](/Api/Classes/GamePlay/Chat_F/SetActorShowEditorChatBubble.md) ([bool](/Api/DataType/Bool.md) actorShowEditorBubble)</div>|
|:---|
|设置角色聊天显示的聊天气泡是否是工具聊天气泡|

## 事件

