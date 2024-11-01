---
{"title":"Local Space Viewer开源地形","dg-publish":true,"dg-note-icon":"2","dg-path":"🌳 Major/Geography/Local Space Viewer 开源地形.md","permalink":"/🌳 Major/Geography/Local Space Viewer 开源地形/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-01T21:42:39.326+08:00"}
---

[[D 📚 RESOURCE/⚒️ Software/geography/Local Space Viewer\|Local Space Viewer]]
国产软件的免费高程信息生成地形
加载卫星地图「百度地图」/「高德地图」/「谷歌地图」
加载地形「三维地形」-「SRTM 3（90 米）. Lrc」
「下载」-「提取高程」-「绘制矩形」采样间距「300」-「提取」-「导出 CSV 格式」
打开 Excel，A 前插入一列，C 剪贴到 A，删除 C，再在 A 前插入一列，删除 1 行，在 A 列输入序号 1、2、3 选中出➕向下拖到末尾。导出为「txt」文件。
导入「谷歌地球取点工具」-「输出」-「转换」-「mapGIS」导入[[D 📚 RESOURCE/⚒️ Software/Rhinoceros 3D/Rhino\|Rhino]]
「DAT 文件转为点阵」电池包拖入[[Grasshopper _基础\|Grasshopper _基础]] 内
右键电池「Select one existing file」选择刚才的「DAT」文件-「标准」-「缩放到最大范围」
框选-「Patch」
取样点间距「1」控制点数
UV「50 50」控制精细程度
硬度「1」越小越贴合
「Top」视图画框，「Trim」裁切掉多余边
向下挤出，「Front」视图画线「Trim」切平
「转换曲面/多重曲面为网格」
「Front」视图下「Contour」等距断面线向上
「挤出封闭的平面曲线」-「实体」点是-长度为等高线高度
「文件」-「导出选取的物件」导出为 SKP 文件到[[D 📚 RESOURCE/⚒️ Software/SketchUp\|SketchUp]]