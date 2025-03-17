# UIModelView

## 属性

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanCameraMove</font></div>|
|:---|
|是否启用视角拖拽（拖拽UI时相机围绕模型旋转）|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CameraDist</font></div>|
|:---|
|相机与原点距离|

|<div style="width:700px">[Button](/Api/Enums/Button.md) &emsp;<font color="dd00dd">ResetCameraBtn</font></div>|
|:---|
|重置相机按钮|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LookAtPosition</font></div>|
|:---|
|锁定相机位置|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CameraLockX</font></div>|
|:---|
|视角拖拽时是否锁定X轴方向|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CameraLockY</font></div>|
|:---|
|视角拖拽时是否锁定Y轴方向|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CameraPitch</font></div>|
|:---|
|相机俯仰角|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">CameraYaw</font></div>|
|:---|
|相机偏航角|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnablePostProcessing</font></div>|
|:---|
|开启后处理|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">BloomActive</font></div>|
|:---|
|全屏泛光是否激活|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">BloomIntensity</font></div>|
|:---|
|全屏泛光强度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">BloomThreshold</font></div>|
|:---|
|全屏泛光阈值|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DofActive</font></div>|
|:---|
|自由度是否激活|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DofFocalRegion</font></div>|
|:---|
|字段焦点区域深度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DofNearTransitionRegion</font></div>|
|:---|
|字段最近转换区域的深度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DofFarTransitionRegion</font></div>|
|:---|
|字段深度转换区域|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DofFocalDistance</font></div>|
|:---|
|景深焦距深度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">DofScale</font></div>|
|:---|
|字段比例深度|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AntialiasingEnable</font></div>|
|:---|
|抗锯齿开启|

|<div style="width:700px">[AntialiasingMethodDesc](/Api/Enums/AntialiasingMethodDesc.md) &emsp;<font color="dd00dd">AntialiasingMethod</font></div>|
|:---|
|抗锯齿方法|

|<div style="width:700px">[AntialiasingQualityDesc](/Api/Enums/AntialiasingQualityDesc.md) &emsp;<font color="dd00dd">AntialiasingQuality</font></div>|
|:---|
|抗锯齿质量|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">LUTsActive</font></div>|
|:---|
|LUTs开启|

|<div style="width:700px">[LUTsTemperatureType](/Api/Enums/LUTsTemperatureType.md) &emsp;<font color="dd00dd">LUTsTemperatureType</font></div>|
|:---|
|LUTs温度类型|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsWhiteTemp</font></div>|
|:---|
|LUTs白色温度|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsWhiteTint</font></div>|
|:---|
|LUTs白色色调|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsColorCorrectionShadowsMax</font></div>|
|:---|
|LUTs最大色彩校正阴影|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsColorCorrectionHighlightsMin</font></div>|
|:---|
|LUTs最小色彩校正高亮|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsBlueCorrection</font></div>|
|:---|
|LUTs蓝光校正|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsExpandGamut</font></div>|
|:---|
|LUTs扩展色域|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsToneCurveAmout</font></div>|
|:---|
|LUTs色调曲线数量|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsFilmicToneMapSlope</font></div>|
|:---|
|LUTs电影色调映射斜率|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsFilmicToneMapToe</font></div>|
|:---|
|LUTs电影色调映射阴影|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsFilmicToneMapShoulder</font></div>|
|:---|
|LUTs电影色调映射高光|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsFilmicToneMapBlackClip</font></div>|
|:---|
|LUTs电影色调映射黑色调|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LUTsFilmicToneMapWhiteClip</font></div>|
|:---|
|LUTs电影色调映射白色调|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsBaseSaturation</font></div>|
|:---|
|LUTs基础饱和颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsBaseContrast</font></div>|
|:---|
|LUTs基础对比颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsBaseGamma</font></div>|
|:---|
|LUTs基础γ颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsBaseGain</font></div>|
|:---|
|LUTs基础增益颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsBaseOffset</font></div>|
|:---|
|LUTs基础偏移颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsShadowSaturation</font></div>|
|:---|
|LUTs阴影饱和颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsShadowContrast</font></div>|
|:---|
|LUTs阴影对比颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsShadowGamma</font></div>|
|:---|
|LUTs阴影γ颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsShadowGain</font></div>|
|:---|
|LUTs阴影增益颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsShadowOffset</font></div>|
|:---|
|LUTs阴影偏移颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsMidtoneSaturation</font></div>|
|:---|
|LUTs中间色调饱和颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsMidtoneContrast</font></div>|
|:---|
|LUTs中间色调对比颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsMidtoneGamma</font></div>|
|:---|
|LUTs中间色调γ颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsMidtoneGain</font></div>|
|:---|
|LUTs中间色调增益颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsMidtoneOffset</font></div>|
|:---|
|LUTs中间色调偏移颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsHighlightSaturation</font></div>|
|:---|
|LUTs高光饱和颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsHighlightContrast</font></div>|
|:---|
|LUTs高光对比颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsHighlightGamma</font></div>|
|:---|
|LUTs高光γ颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsHighlightGain</font></div>|
|:---|
|LUTs高光增益颜色|

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">LUTsHighlightOffset</font></div>|
|:---|
|LUTs高光偏移颜色|

|<div style="width:700px">[ModelAssetType](/Api/DataType/ModelAssetType.md) &emsp;<font color="dd00dd">LUTsColorGradingLUTPath</font></div>|
|:---|
|LUTs颜色分级表路径|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">GTAOActive</font></div>|
|:---|
|GTAO开关|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOThicknessblend</font></div>|
|:---|
|0~1|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOFalloffStartRatio</font></div>|
|:---|
|0-1|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOFalloffEnd</font></div>|
|:---|
|0-300|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOFadeoutDistance</font></div>|
|:---|
|0-20000|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOFadeoutRadius</font></div>|
|:---|
|0-10000|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOIntensity</font></div>|
|:---|
|0-1|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">GTAOPower</font></div>|
|:---|
|0-10|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ChromaticAberrationActive</font></div>|
|:---|
|开关|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ChromaticAberrationIntensity</font></div>|
|:---|
|0-8|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ChromaticAberrationStartOffset</font></div>|
|:---|
|0-1|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ChromaticAberrationIterationStep</font></div>|
|:---|
|0.01-10|

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ChromaticAberrationIterationSamples</font></div>|
|:---|
|1-8|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">DisEnableDefaultLight</font></div>|
|:---|
|是否关闭默认光照|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">SkyLight</font></div>|
|:---|
||

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">SkyLightCubeAssetID</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SkyLightIntensity</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">SkyLightColor</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SkyLightBlendAmount</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">SkyLightAmbientSkyColor</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">SkyLightAmbientEquatorColor</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">SkyLightAmbientGroundColor</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">SkyLightAmbientColor</font></div>|
|:---|
||

|<div style="width:700px">[MODELVIEW_FogType](/Api/Enums/MODELVIEW_FogType.md) &emsp;<font color="dd00dd">FogType</font></div>|
|:---|
||

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">FogColor</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FogStart</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">FogEnd</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Atmosphere</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">LightEuler</font></div>|
|:---|
||

|<div style="width:700px">[float](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LightIntensity</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">LightActive</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EnableShadow</font></div>|
|:---|
||

|<div style="width:700px">[UIMODLEVIEW_SkyLightType](/Api/Enums/UIMODLEVIEW_SkyLightType.md) &emsp;<font color="dd00dd">SkyLightType</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ResetCamera</font> ()</div>|
|:---|
|重置相机|

## 代码示例

```lua
--创建ui布局
local root = SandboxNode.new('UIRoot', game.WorkSpace)
root.Name = 'uiroot'

--创建UI
local ModelView = SandboxNode.new('UIModelView', game.WorkSpace.uiroot)
ModelView.Size = Vector2.new(500, 500)
ModelView.Position = Vector2.new(500, 500)
ModelView.CanCameraMove = true
ModelView.CameraDist = 700

local newModel= SandboxNode.new('Model')
newModel.Name = "my_model"
newModel.ModelId = "sandboxSysId://entity/100011/body.omod"
newModel.Position = Vector3.new(0,0,0)
--设置父节点 将模型节点添加到ModelView中
newModel:SetParent(ModelView)
```