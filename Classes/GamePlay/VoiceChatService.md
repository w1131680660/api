# VoiceChatService

## 属性

|<div style="width:700px">[ChannelType](/Api/Enums/ChannelType.md) &emsp;<font color="dd00dd">ChannelType</font></div>|
|:---|
|语音频道类型|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsSingleChannel</font>](/Api/Classes/GamePlay/VoiceChatService_F/IsSingleChannel.md) ([bool](/Api/DataType/Bool.md) bCheck)</div>|
|:---|
|是否单频道|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">JoinVoiceChannel</font>](/Api/Classes/GamePlay/VoiceChatService_F/JoinVoiceChannel.md) ([int](/Api/DataType/Number.md) uin, [CHANNEL_ID](/Api/Enums/CHANNEL_ID.md) channelID)</div>|
|:---|
|加入某语音频道|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">AssignVoiceChannel</font>](/Api/Classes/GamePlay/VoiceChatService_F/AssignVoiceChannel.md) ([int](/Api/DataType/Number.md) uin, [CHANNEL_ID](/Api/Enums/CHANNEL_ID.md) channelID)</div>|
|:---|
|分配某语音频道|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">QuitVoiceChannel</font>](/Api/Classes/GamePlay/VoiceChatService_F/QuitVoiceChannel.md) ([int](/Api/DataType/Number.md) uin, [CHANNEL_ID](/Api/Enums/CHANNEL_ID.md) channelID)</div>|
|:---|
|退出某语音频道|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">QuitAllVoiceChannel</font>](/Api/Classes/GamePlay/VoiceChatService_F/QuitAllVoiceChannel.md) ([int](/Api/DataType/Number.md) uin)</div>|
|:---|
|退出所有语音频道|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSpeakerStatus</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetSpeakerStatus.md) ([int](/Api/DataType/Number.md) uin, [bool](/Api/DataType/Bool.md) bActive)</div>|
|:---|
|设置扬声器状态|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetSpeakerStatus</font>](/Api/Classes/GamePlay/VoiceChatService_F/GetSpeakerStatus.md) ([int](/Api/DataType/Number.md) uin)</div>|
|:---|
|获取扬声器状态|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMicroPhoneStatus</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetMicroPhoneStatus.md) ([int](/Api/DataType/Number.md) uin, [bool](/Api/DataType/Bool.md) bActive)</div>|
|:---|
|设置麦克风状态|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetMicroPhoneStatus</font>](/Api/Classes/GamePlay/VoiceChatService_F/GetMicroPhoneStatus.md) ([int](/Api/DataType/Number.md) uin)</div>|
|:---|
|获取麦克风状态|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetVolume</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetVolume.md) ([int](/Api/DataType/Number.md) uin, [int](/Api/DataType/Number.md) val)</div>|
|:---|
|调节音量|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetVolume</font>](/Api/Classes/GamePlay/VoiceChatService_F/GetVolume.md) ([int](/Api/DataType/Number.md) uin)</div>|
|:---|
|获取音量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetListenOther</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetListenOther.md) ([int](/Api/DataType/Number.md) setUin, [int](/Api/DataType/Number.md) otherUin, [bool](/Api/DataType/Bool.md) bListen)</div>|
|:---|
|聆听他人|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">MicroPhoneSwitchBtn</font> ()</div>|
|:---|
|麦克风开关按钮|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SpeakerSwitchBtn</font> ()</div>|
|:---|
|扬声器开关按钮|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">QuitAllVoiceChannelClient</font> ()</div>|
|:---|
|退出所有语音频道|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetSpeakerStatusClient</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetSpeakerStatusClient.md) ([bool](/Api/DataType/Bool.md) arg1)</div>|
|:---|
|设置扬声器状态(客户端方法)|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetSpeakerStatusClient</font>](/Api/Classes/GamePlay/VoiceChatService_F/GetSpeakerStatusClient.md) ()</div>|
|:---|
|获取扬声器状态(客户端方法)|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetMicroPhoneStatusClient</font>](/Api/Classes/GamePlay/VoiceChatService_F/SetMicroPhoneStatusClient.md) ([bool](/Api/DataType/Bool.md) arg1)</div>|
|:---|
|设置麦克风状态(客户端方法)|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetMicroPhoneStatusClient</font>](/Api/Classes/GamePlay/VoiceChatService_F/GetMicroPhoneStatusClient.md) ()</div>|
|:---|
|获取麦克风状态(客户端方法)|

