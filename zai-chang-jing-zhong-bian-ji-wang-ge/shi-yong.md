# 使用

1. 打开测试场景，在工程目录/Assets/XSGridEditor/Scene/Demo\_1.unity
2. 编辑器里关掉TextMeshPro的图标显示，不然太多看不清，方法为 ：点击Scene面板上方的Gizmos，点击TextMeshPro的图标让它变暗
3. 设置画板画笔：从菜单栏 Window->2D->Tile Palette打开窗口，切记上方Active Tilemap选择Tilemap；下方Default Brush改为GameObject BrushEx（或者下面那个GameObject Brush），点开Cells->Element 0->GameObject选择Quad这个prefab
4. 画tile时会自动让调整自己的y使得贴在Terrian上，如果地表有装饰物，那tile还会自动贴在装饰物的上面
5. quad这个perfab上挂了个XSGridData组件，用来单独设置tile属性的
