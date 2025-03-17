# UIBMLabel

## 属性

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BMText</font></div>|
|:---|
|文本内容|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BMFonts</font></div>|
|:---|
|字体|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BMPng</font></div>|
|:---|
|资源|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TargetID</font></div>|
|:---|
|跟随目标|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Grayed</font></div>|
|:---|
|置灰|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Animable</font></div>|
|:---|
|支持动画|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Offset</font></div>|
|:---|
||

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">Alpha</font></div>|
|:---|
|透明度|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">BMColor</font></div>|
|:---|
|文本颜色|

|<div style="width:700px">[BMGradientDirType](/Api/Enums/BMGradientDirType.md) &emsp;<font color="dd00dd">GradientDir</font></div>|
|:---|
|渐变色起始色|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GradientOrigin</font></div>|
|:---|
||

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GradientTarget</font></div>|
|:---|
||

## 成员函数

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetLabelNum</font>](/Api/Classes/Other/UIBMLabel_F/GetLabelNum.md) ()</div>|
|:---|
|获取Label数量|

|<div style="width:700px">[SandboxNode](/Api/Classes/Base/SandboxNode.md) &emsp;[<font color="dd00dd">GetLabel</font>](/Api/Classes/Other/UIBMLabel_F/GetLabel.md) ()</div>|
|:---|
|获取第N个Label节点|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">SetLoadedCallback</font>](/Api/Classes/Other/UIBMLabel_F/SetLoadedCallback.md) ([LuaFunction](/Api/Enums/LuaFunction.md) arg1)</div>|
|:---|
|纹理字加载完成|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">FollowTarget</font>](/Api/Classes/Other/UIBMLabel_F/FollowTarget.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) arg1)</div>|
|:---|
|跟随对象|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local root = SandboxNode.new('UIRoot', workspace)
local label = SandboxNode.new('UIBMLabel', root)
local loadedFun = function(status, asset)

end
label:SetLoadedCallback(loadedFun)
label.BMText = "123"
label.BMFonts = "sandboxId://miniui/miniworld/defaultBM.fnt"
label.BMPng = "sandboxId://miniui/miniworld/defaultBM.png"
label.Position = Vector2.new(100, 100)
label.Scale = Vector2.new(0.8, 0.8)
label.Alpha = 255
label:FollowTarget(workspace.Model)
```