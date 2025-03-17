# UIDropDownBox

## 属性

|<div style="width:700px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TitleColor</font></div>|
|:---|
|文本颜色|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TitleFontSize</font></div>|
|:---|
|文本字体大小|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">SelectedIndex</font></div>|
|:---|
|选中的下标|

## 成员函数

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetValue</font>](/Api/Classes/Scene/UIDropDownBox_F/GetValue.md) ()</div>|
|:---|
|获取下拉框选中的内容|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetItem</font>](/Api/Classes/Scene/UIDropDownBox_F/GetItem.md) ()</div>|
|:---|
|获取下拉框某item项|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">AddItemWithValue</font>](/Api/Classes/Scene/UIDropDownBox_F/AddItemWithValue.md) ([string](/Api/DataType/String.md) item, [string](/Api/DataType/String.md) value)</div>|
|:---|
|给下拉框新增一项item|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">AddItem</font>](/Api/Classes/Scene/UIDropDownBox_F/AddItem.md) ([string](/Api/DataType/String.md) item)</div>|
|:---|
|给下拉框添加一项item|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">RemoveItem</font>](/Api/Classes/Scene/UIDropDownBox_F/RemoveItem.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|通过下标移除下拉框中某项item|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetItemByIndex</font>](/Api/Classes/Scene/UIDropDownBox_F/GetItemByIndex.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|通过下标获取下拉框中某项item的key|

|<div style="width:700px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetValueByIndex</font>](/Api/Classes/Scene/UIDropDownBox_F/GetValueByIndex.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|通过下标获取下拉框中某项item的value|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetIndexByItem</font>](/Api/Classes/Scene/UIDropDownBox_F/GetIndexByItem.md) ([string](/Api/DataType/String.md) )</div>|
|:---|
||

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">SelectIndexChange</font>](/Api/Classes/Scene/UIDropDownBox_F/SelectIndexChange.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [int](/Api/DataType/Number.md) index)</div>|
|:---|
|索引切换事件|

