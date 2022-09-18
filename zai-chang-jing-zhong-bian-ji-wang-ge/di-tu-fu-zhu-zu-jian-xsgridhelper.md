# 地图辅助组件 XSGridHelper

这个组件挂在了Grid节点上，有几个按钮，如图1所示：

![图1](../.gitbook/assets/v2-985515611b7aa2b8b7c5027cfc79ad17\_720w.png)

用处分别如下

### 1.tile贴到地面

画tile时如果没有自动设置高度，可以点击这个全部统一设置。

### 2.显示tile坐标

在tile上显示坐标，debug用

### 3.显示tile移动消耗

在tile上显示移动消耗，读取的XSGridData的Cost参数

### 4.删除所有tile

gameobject brush好像没法批量删除，点这个可以全部删除

### 5.创建1个XSObject

创建1个单位对象在0，0的位置，鼠标拖动到其他格子就算设置它的网格位置了，填的id是你数据表里单位的id
