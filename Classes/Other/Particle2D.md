# Particle2D

## 属性

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">AssetID</font></div>|
|:---|
|plist资源id|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Duration</font></div>|
|:---|
|-1表示无限长|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Life</font></div>|
|:---|
|-1表示无限长|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LifeVar</font></div>|
|:---|
|单位秒|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartSize</font></div>|
|:---|
|粒子初始大小|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartSizeVar</font></div>|
|:---|
|粒子初始大小变化率|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EndSize</font></div>|
|:---|
|粒子结束大小|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EndSizeVar</font></div>|
|:---|
|粒子结束大小变化率|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Angle</font></div>|
|:---|
|粒子初始角度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartSpin</font></div>|
|:---|
|粒子初始旋转速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EndSpin</font></div>|
|:---|
|粒子结束旋转速度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EmissionRate</font></div>|
|:---|
|粒子发射速率|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">StartColor</font></div>|
|:---|
|设置粒子初始颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">StartColorVar</font></div>|
|:---|
|设置粒子初始颜色变化率|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">EndColor</font></div>|
|:---|
|设置粒子结束颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">EndColorVar</font></div>|
|:---|
|设置粒子结束颜色变化率|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">TexAssetID</font></div>|
|:---|
|纹理资源id|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">StartSpinVar</font></div>|
|:---|
|设置粒子初始旋转速度变化率|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">EndSpinVar</font></div>|
|:---|
|设置粒子结束旋转速度变化率|

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetTexAssetID</font>](/Api/Classes/Other/Particle2D_F/SetTexAssetID.md) ([ModelAssetType](/Api/DataType/ModelAssetType.md) assetID, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置资源id|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetAssetID</font>](/Api/Classes/Other/Particle2D_F/SetAssetID.md) ([ModelAssetType](/Api/DataType/ModelAssetType.md) assetID, [LuaFunction](/Api/Enums/LuaFunction.md) callback)</div>|
|:---|
|设置plist资源id|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Play</font> ()</div>|
|:---|
|播放暂停的特效|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Stop</font> ()</div>|
|:---|
|停止特效|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ReStart</font> ()</div>|
|:---|
|重新播放特效|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">Pause</font> ()</div>|
|:---|
|暂停特效|

