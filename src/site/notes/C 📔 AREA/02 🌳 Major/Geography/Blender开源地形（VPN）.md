---
{"title":"Blender开源地形（VPN）","dg-publish":true,"dg-note-icon":"2","dg-path":"🌳 Major/Geography/Blender开源地形（VPN）.md","permalink":"/🌳 Major/Geography/Blender开源地形（VPN）/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-01T21:42:39.328+08:00"}
---

利用 blenderGIS 插件在 Blender 里获取地形和建筑体快

**插件安装**

「编辑」-「偏好设置」-「插件」-「安装」-找到压缩包，无需解压

**获取地图**

「GIS」-「Web geodata」-「Basemap」源选「Esri」

「G」搜索-放大级别「16」

**获取地形**

「E」锁定-选中图片-「GIS」-「Web geodata」-「Get elevation（SRTM）」

**获取建筑体块**

选中图片-「GIS」-「Web geodata」-「Get OSM」-「building」可加选其他-勾选「Elevation from object」

**导出**

导出 obj 导入 [[D 📚 RESOURCE/⚒️ Software/Rhinoceros 3D/Rhino\|Rhino]] -勾选「映射 OBJ 的 Y 方向到 Rhino 的 Z 方向」