---
{"title":"SU开源地形（VPN）","dg-publish":true,"dg-note-icon":"2","dg-path":"🌳 Major/Geography/SU开源地形（VPN）.md","permalink":"/🌳 Major/Geography/SU开源地形（VPN）/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-01T21:42:39.314+08:00"}
---

注册一个SketchUp账号，「文件」-「地理位置」-「添加位置」
「选择区域」-「Digital Globe」-「导入」
重复上面步骤可以导入多个图片并自动拼合，切记两张照片不能距离太远
导入[[D 📚 RESOURCE/⚒️ Software/Rhinoceros 3D/Rhino\|Rhino]] 「导入为修剪过的平面」
「SU 曲面捕捉点」电池包拖入[[Grasshopper _基础\|Grasshopper _基础]] 内。启动电池包，鼠标中键点击「Suface」-「Bake」_（付费课程资料）_
炸开-「ungroup」解组，选择电池右键「Set Multiple Surface」-鼠标中键「Bake」得到高程点
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