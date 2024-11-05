---
{"tags":["software"],"type":["GIS","地理信息","地图"],"dg-publish":true,"dg-note-icon":"1","dg-path":"⚒️ Software/geography/Esri_ArcGIS.md","permalink":"/⚒️ Software/geography/Esri_ArcGIS/","dgPassFrontmatter":true,"noteIcon":"1","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-05T23:48:11.659+08:00"}
---

# Setting 设置  
-   自定义 arcmap选项 滚轮 放大  
-   打开「ArcToolbox」「目录」「Search」  
-   右键图层-属性可查看坐标系  
# Tool 工具  
-   「Mosaic to new raster」镶嵌至新的栅格  
	-   多张图拼合为1张![](https://api2.mubu.com/v3/document_image/ccd34496-6835-4991-ae61-2096a0466135-20454557.jpg)  
	-   输置建立一个数据库注意命名  
	-   像素类型  
		-   2的N次方一般16 BIT UNSIGNED  
	-   波段数1  
-   「Project raster」投影栅格  
	-   改变栅格的投影坐标系![](https://api2.mubu.com/v3/document_image/9f797ebd-45a1-4df6-b39a-57c6a9515de6-20454557.jpg)  
	-   填写该地区的投影坐标系  
-   「Copy raster」复制栅格  
	-   裁剪范围![](https://api2.mubu.com/v3/document_image/39d0aec2-4f86-4432-ace1-7f9736a53e69-20454557.jpg)  
	-   环境-处理范围-窗口  
-   「Contour」等值线「con」  
	-   生成等高线![](https://api2.mubu.com/v3/document_image/213cd7b9-73d1-47c4-aa29-8b8ab4320b1b-20454557.jpg)  
-   「Focal Statistics」焦点统计「fsc」  
	-   为每个输入像元位置计算其周围指定领域内的值的统计数据![](https://api2.mubu.com/v3/document_image/be7d72b4-8cc4-4bc7-9543-6f2f441a97a3-20454557.jpg)  
	-   柔化图像增加高程顺滑度损失高程精度  
	-   领域分析-圆形  
	-   半径5  
	-   统计类型MEAN  
-   「Resample」重采样「re」  
	-   细化单元像素格增加细节程度损失高程精度![](https://api2.mubu.com/v3/document_image/3d1af371-fe06-4e16-9ff6-606d143ab510-20454557.jpg)  
	-   适合做小尺度地形对系统要求高  
	-   y坐标小数点向左移一位  
-   「Slope」坡度分析「sl」  
-   「Aspect」坡向分析「as」  
# 水文分析  
-   「Fill」填洼  
	-   环境并行处理0  
-   「Flow Direction」流向 「fd」  
	-   环境并行处理0  
-   「Flow Accumulation」流量「acc」  
	-   输出数据类型INTEGER  
-   「stream to feature」栅格河网矢量化 「stf」  
-   「Basin」盆域分析 「bas」  
-   「Raster Calculator」栅格计算器 「cal」  
	-   语句  
		-   Co(条件，条件成立输出的值条件不成立输出的值条件语句  
-   「Raster to Polygon」栅格转面 「rtp」