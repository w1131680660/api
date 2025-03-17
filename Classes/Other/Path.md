# Path

## 成员函数

|<div style="width:700px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GeneratePaths</font>](/Api/Classes/Other/Path_F/GeneratePaths.md) ([Vector3](/Api/DataType/Vector3.md) start, [Vector3](/Api/DataType/Vector3.md) finish)</div>|
|:---|
|同步生成路径|

|<div style="width:700px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">GetPaths</font>](/Api/Classes/Other/Path_F/GetPaths.md) ()</div>|
|:---|
|获取生成的路径|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">GenerateNavMeshAsync</font> ()</div>|
|:---|
|异步生成导航网格,并持续持有,不会被释放。|

|<div style="width:700px">[void](/Api/DataType/Void.md) &emsp;<font color="dd00dd">ClearNavMesh</font> ()</div>|
|:---|
|清理导航网格,不再继续持有,随系统定期gc释放|

