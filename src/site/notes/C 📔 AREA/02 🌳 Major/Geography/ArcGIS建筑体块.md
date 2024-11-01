---
{"title":"ArcGIS建筑体块","dg-publish":true,"dg-note-icon":"2","dg-path":"🌳 Major/Geography/ArcGIS建筑体块.md","permalink":"/🌳 Major/Geography/ArcGIS建筑体块/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-01T21:42:39.329+08:00"}
---

最强的数据获得方法，前提是有 shp 文件
**获取 [[C 📔 AREA/02 🌳 Major/Geography/Data Tpye/SHP\|SHP]] 数据**
-   找代下
-   淘宝
-   水经注
-   「百度建筑（含高度）」
-   右上角地名下载
-   顶上「下载」框选区域
-   坐标投影「西安 80 高斯投影」
**生成建筑体块**
打开「ArcScene」-「目录」链接到 shp 根目录自动识别-导入 shp 文件
「内容列表」-双击「shp 文件」-「拉伸」-打勾「拉伸土层中的要素」-「计算机图标」-「height」
双击正方形可以改颜色
**转换**
「目录」-「工具箱」-「系统工具箱」-「3 D Analyst Tools. Tbx」-「转换」-「3 D 图层转要素类」-输入 shp-可以改输出位置
**导出**
右键「shp 文件」-「编辑要素」-「开始编辑」
右键「shp 文件」-「属性表」-「Ctrl+A」全选-「3 D 编辑器」-「合并」-「停止编辑」-「是」
「目录」-「工具箱」-「系统工具箱」-「Conversion Tools. Tbx」-「转为 Collada」-输入 shp-输出 dae 格式
可导入 [[D 📚 RESOURCE/⚒️ Software/SketchUp\|SketchUp]]