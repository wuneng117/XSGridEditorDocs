# GridMgr

这个类包含了1个PathFinder类的实例对象，并提供了以下功能：

* 世界坐标转网格坐标
* 网格坐标转世界坐标
* 从世界坐标获取网格
* 从网格坐标获取网格
* 世界坐标转网格坐标并获取网格中心后转为世界坐标



```csharp
/// <summary> tile 管理类接口，负责tile 坐标转化，数据等功能 </summary>
    public interface IGridMgr
    {
        /// <summary> 寻路类，同时也存放 tile 的结构数据 PathFinderTile </summary>
        PathFinder PathFinder { get; }

        /// <summary>
        /// 从 tilePos 转为 worldPos
        /// </summary>
        /// <param name="tilePos">表示每个 tile 的坐标</param>
        Vector3 TileToWorld(Vector3Int tilePos);

        /// <summary>
        /// 从 worldPos 转为 tilePos
        /// </summary>
        /// <param name="worldPos">unity 的世界坐标</param>
        Vector3Int WorldToTile(Vector3 worldPos);

        /// <summary>
        /// 从 worldPos 获取tile
        /// </summary>
        /// <param name="worldPos">unity 的世界坐标</param>
        PathFinderTile GetTile(Vector3 worldPos);

        /// <summary>
        /// 从  tilePos 获取 tile
        /// </summary>
        /// <param name="tilePos">表示每个 tile 的坐标</param>
        PathFinderTile GetTile(Vector3Int tilePos);

        /// <summary>
        /// 获取随意一点世界坐标对应 tile 的中心位置
        /// </summary>
        /// <param name="worldPos">unity 的世界坐标</param>
        Vector3 WorldToTileCenterWorld(Vector3 worldPos);C
    }
```

