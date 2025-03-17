# InputObject

## 属性

|<div style="width:700px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Delta</font></div>|
|:---|
|时间增量|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|鼠标相关的事件中，描述鼠标的位置|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">KeyCode</font></div>|
|:---|
|按键事件触发时，对应的按键码，等于枚举UserInputKeyCode中的某个值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">UserInputState</font></div>|
|:---|
|描述输入状态（开始，结束等）等于枚举UserInputState中的某个值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">UserInputType</font></div>|
|:---|
|等于枚举UserInputType中的某个值|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;<font color="dd00dd">TouchId</font></div>|
|:---|
|触摸事件触发|

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsModifierKeyDown</font>](/Api/Classes/Input/InputObject_F/IsModifierKeyDown.md) ([int](/Api/DataType/Number.md) vkey)</div>|
|:---|
|按键是否按下|

|<div style="width:700px">[int](/Api/DataType/Number.md) &emsp;[<font color="dd00dd">GetTouchCount</font>](/Api/Classes/Input/InputObject_F/GetTouchCount.md) ()</div>|
|:---|
|获取触摸次数|

|<div style="width:700px">[ReflexMap](/Api/Enums/ReflexMap.md) &emsp;[<font color="dd00dd">GetTouch</font>](/Api/Classes/Input/InputObject_F/GetTouch.md) ([int](/Api/DataType/Number.md) index)</div>|
|:---|
|获取触摸事件|

