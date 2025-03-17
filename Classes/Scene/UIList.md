# UIList

## 属性

|<div style="width:700px">[OverflowType](/Api/Enums/OverflowType.md) &emsp;<font color="dd00dd">OverflowType</font></div>|
|:---|
|溢出处理，设置ScrollType时，需要将该属性同步修改（如设置横向流动，此处需设置HORIZONTAL）才能达到效果|

|<div style="width:700px">[ListLayoutType](/Api/Enums/ListLayoutType.md) &emsp;<font color="dd00dd">ScrollType</font></div>|
|:---|
|排列方式，需要与OverflowType配套使用才有效果|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LineCount</font></div>|
|:---|
|行数|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ColumnCount</font></div>|
|:---|
|列数|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">LineGap</font></div>|
|:---|
|行距|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">ColumnGap</font></div>|
|:---|
|列距|

|<div style="width:700px">[TextHAlignment](/Api/Enums/TextHAlignment.md) &emsp;<font color="dd00dd">HorizontalAlign</font></div>|
|:---|
|水平对齐方式|

|<div style="width:700px">[TextVAlignment](/Api/Enums/TextVAlignment.md) &emsp;<font color="dd00dd">VerticalAlign</font></div>|
|:---|
|垂直对齐方式|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AutoResizeItem</font></div>|
|:---|
|自动调整列表项目大小，如果勾选:列表布局为单列，则列表项目的宽度自动设置为列表显示区域的宽度；列表布局为单行，则列表项目的高度自动设置为列表显示区域的高度；列表布局为水平流动，且设置了列数时，则每行内的列表项目的宽度自动调整使行宽与列表显示区域的宽度相等；列表布局为垂直流动，且设置了行数时，则每列内的项目的高度自动调整使行高与列表显示区域的高度相等；列表布局为分页，则3、4规则均适用;|

|<div style="width:700px">[Vector4](/Api/DataType/Vector4.md) &emsp;<font color="dd00dd">Padding</font></div>|
|:---|
|边界值|

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ScrollPercent</font></div>|
|:---|
||

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">FoldInvisibleItems</font></div>|
|:---|
|Item隐藏时是否取消预留空位|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Bounceback</font></div>|
|:---|
||

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ContentSize</font></div>|
|:---|
|获取内容大小|

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ScrollItemToViewOnClick</font></div>|
|:---|
|点击item是否显示全|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetVirtual</font>](/Api/Classes/Scene/UIList_F/SetVirtual.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) arg1)</div>|
|:---|
|设置虚拟列表，只为可视范围内的item创建实体对象（不可取消）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetVirtualAndLoop</font> ()</div>|
|:---|
|设置循环列表（同时也是虚拟列表），头尾相接（不可取消）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">SetVirtualItemNum</font> ()</div>|
|:---|
||

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToTop</font>](/Api/Classes/Scene/UIList_F/ScrollToTop.md) ([bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到顶部（允许垂直滚动时可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToBottom</font>](/Api/Classes/Scene/UIList_F/ScrollToBottom.md) ([bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到底部（允许垂直滚动时可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToLeft</font>](/Api/Classes/Scene/UIList_F/ScrollToLeft.md) ([bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到最左边（允许水平滚动时可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToRight</font>](/Api/Classes/Scene/UIList_F/ScrollToRight.md) ([bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到最右边（允许水平滚动时可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToView</font>](/Api/Classes/Scene/UIList_F/ScrollToView.md) ([int](/Api/DataType/Number.md) , [bool](/Api/DataType/Bool.md) arg2, [bool](/Api/DataType/Bool.md) arg3)</div>|
|:---|
|滚动到list某一个项|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToPercentX</font>](/Api/Classes/Scene/UIList_F/ScrollToPercentX.md) ([float](/Api/DataType/Number.md) value, [bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到水平百分比位置（允许水平滚动时可用）|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;[<font color="dd00dd">ScrollToPercentY</font>](/Api/Classes/Scene/UIList_F/ScrollToPercentY.md) ([float](/Api/DataType/Number.md) value, [bool](/Api/DataType/Bool.md) ani)</div>|
|:---|
|滚动到垂直百分比位置（允许垂直滚动时可用）|

## 事件

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyItemRefresh</font>](/Api/Classes/Scene/UIList_F/NotifyItemRefresh.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node, [int](/Api/DataType/Number.md) index)</div>|
|:---|
|Item刷新内容通知|

|<div style="width:700px">[SBXSignal](/Api/DataType/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyItemRegister</font>](/Api/Classes/Scene/UIList_F/NotifyItemRegister.md) ([SandboxNode](/Api/Classes/Base/SandboxNode.md) node)</div>|
|:---|
|Item注册通知|

## 代码示例

```lua
local workspace = game:GetService("WorkSpace")
local name = SandboxNode.new('UIList', workspace)

--设置排列方式
name.ScrollType = Enum.ListLayoutType.FLOW_HORIZONTAL
name.OverflowType = Enum.OverflowType.HORIZONTAL
--设置行数列数
name.LineCount = 2
name.ColumnCount = 2

--设置行距列距
name.LineGap= 50
name.ColumnGap= 50

--设置自动调整项目大小
name.AutoResizeItem= true

--设置上下居中对齐
name.HorizontalAlign= Enum.TextVAlignment.Center
--设置左右向左对齐
name.VerticalAlign= Enum.TextHAlignment.Left

--设置虚拟循环列表
name.SetVirtualAndLoop
```