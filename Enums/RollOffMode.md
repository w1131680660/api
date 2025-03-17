# RollOffMode

------------------------------------------------------------------------------------------
## 描述

声音衰减模式

------------------------------------------------------------------------------------------
## 枚举

|<div style="width:200px">RollOffMode</div>|<div style="width:100px"></div>|<div style="width:100px"></div>|
|:---|:---|:---|
|**名称**|**值**|**描述**|
|Inverse|1|该声音将遵循逆衰减模型，其中mindistance=全音量，maxdistance=声音停止衰减，衰减根据全局衰减系数|
|Linear|2|该声音将遵循线性衰减模型，其中mindistance=全音量，maxdistance=静音|
|LinearSquare|3|该声音将遵循线性平方衰减模型，其中mindistance=全音量，maxdistance=静音|
|InverseTapered|4|在距离接近mindistance时，该声音将遵循逆衰减模型，在距离接近maxdistance的情况下，该声音会遵循线性平方衰减模型|
