# AssetContent

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Ready</font>](/Api/Classes/Cloud/AssetContent_F/Ready.md) ()</div>|
|:---|
|是否准备就绪|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">Load</font>](/Api/Classes/Cloud/AssetContent_F/Load.md) ([AssetResType](/Api/Enums/AssetResType.md) loadType, [string](/Api/DataType/String.md) assetId)</div>|
|:---|
|通过资源类型和id加载该资源|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Clear</font> ()</div>|
|:---|
|该资源清除|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsLoadSuccess</font>](/Api/Classes/Cloud/AssetContent_F/IsLoadSuccess.md) ()</div>|
|:---|
|该资源模型是否已经加载完成|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetLoadAssetId</font>](/Api/Classes/Cloud/AssetContent_F/GetLoadAssetId.md) ()</div>|
|:---|
|获取加载的资源id|

|<div style="width:700px">[AssetResType](/Api/Enums/AssetResType.md) &emsp;[<font color="dd00dd">GetResType</font>](/Api/Classes/Cloud/AssetContent_F/GetResType.md) ()</div>|
|:---|
|获取加载的资源类型|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">LoadFinish</font>](/Api/Classes/Cloud/AssetContent_F/LoadFinish.md) ([bool](/Api/DataType/Bool.md) isFinish)</div>|
|:---|
|资源加载完成时触发|

