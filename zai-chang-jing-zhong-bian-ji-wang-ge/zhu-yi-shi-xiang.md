# 注意事项

* 切记上方Active Tilemap选择Tilemap，否则会画到其他节点上导致显示错误，也无法被认定为tile
* 橡皮擦有时候擦不掉，可能tile的scale和画笔的cells的不一样，只能手动选择删除；橡皮擦也不能批量删除
* 下方的GameObjectBrushEx的Cells的长度是通过设置Size来改变的，而且不是用来设置多个tile当画板用的！基本没什么用处吧。。。实际功能是：比如Size设置x和y都是2，然后Cells里设置好4个element，那你就可以一次画正方形的4个element，类似在画板里选择多个tile来画占多个格子的东西。
* 如何设置tile的大小：首先Grid组件的CellSize设置成你要的大小，然后同样设置GameObjectBrushEx里的Element的Scale，不需要修改prefab
