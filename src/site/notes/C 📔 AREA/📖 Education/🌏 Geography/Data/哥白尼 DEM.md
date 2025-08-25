---
{"dg-publish":true,"permalink":"/C 📔 AREA/📖 Education/🌏 Geography/Data/哥白尼 DEM/","noteIcon":"stone","created":"2025-08-16T13:55:22.781+08:00","updated":"2024-11-05T23:56:13.335+08:00"}
---

数字高程模型 (Digital Elevation Model, DEM)是地球表面高程起伏的数字化表示，随着越来越多的光学立体测绘卫星和干涉雷达卫星发射升空，可用的全球性和区域性的 DEM 数据集数量也在不断增长。全球性的开源 DEM 数据集有 ETOPO、GTOPO30、GMTED2010、SRTM DEM、NASA DEM、ASTER GDEM、AW3D30、TanDEM-X DEM、Copernicus DEM 等。全球性的开源 DEM 数据集由于免费和可以开放使用受到大家的广泛欢迎。
哥白尼DEM(Copernicus DEM)是公认的最佳全球性开源DEM之一，我个人认为可以去掉之一，有以下几个原因：**（1）绝对高程精度和水平精度在全球性的开源DEM中最佳**；**（2）该DEM的现势性是最好**的，生产DEM的数据采集自2010-2015年；**（3）地形细节表现最佳**，该DEM由高分辨率的DEM抽样成30米格网间距，纸面上格网间距指标虽然与NASA DEM、AW3D等一致，但实际效果优于30米分辨率；**（4）无法量化的影响DEM使用的细节最佳**，该DEM由经过了人工编辑的高分辨率DEM抽样得到，一致性更好。  
在前续一系列文章中已对哥白尼DEM和开源DEM有过介绍：[开源DEM指南v1.0](https://link.zhihu.com/?target=http%3A//mp.weixin.qq.com/s%3F__biz%3DMzk0MDQzNTEyNg%3D%3D%26mid%3D2247485084%26idx%3D1%26sn%3D7c9a66ff95a198492b8618f596dfac45%26chksm%3Dc2e0f545f5977c5327f9895f19a73bb63ae9431628612f913a2c72408ed2a2d0661d4e323ce4%26scene%3D21%23wechat_redirect)、[数据分享-精准地形数据哥白尼DEM(30米)中国区域分块镶嵌](https://link.zhihu.com/?target=http%3A//mp.weixin.qq.com/s%3F__biz%3DMzk0MDQzNTEyNg%3D%3D%26mid%3D2247485455%26idx%3D1%26sn%3Dfe0c3539896498b7a4ff9bdfe5c7b95a%26chksm%3Dc2e0fbd6f59772c046f2d9cc7efbf3e5dcd8a3dd8c32a9ad484128a009ec4f337658f65b30ff%26scene%3D21%23wechat_redirect)、[ALOS 12.5米DEM(数字高程模型)“名不符实”](https://link.zhihu.com/?target=http%3A//mp.weixin.qq.com/s%3F__biz%3DMzk0MDQzNTEyNg%3D%3D%26mid%3D2247484743%26idx%3D1%26sn%3D334d39b73b941883d42e8ca9d668bbcd%26chksm%3Dc2e0f69ef5977f88907cc01246eabfe37d497d9c6fd087f21b3030ba92f33865bde4f45b814e%26scene%3D21%23wechat_redirect)。但是还是有不少人发信问跟哥白尼DEM相关的一些问题，比如哥白尼DEM和TanDEM-X DEM的关系、哥白尼DEM做了哪些编辑、30米的格网间距为什么会有这么高的水平精度？等等。这篇文章对哥白尼DEM进行了较为详细的介绍，可以回答上述问题。  
**一、概述**
哥白尼数字高程模型(Copernicus DEM, COP-DEM)由欧洲航天局(European Space Agency, 简称ESA或欧空局)发布，全球范围免费提供30米和90米分辨率DEM。COP-DEM是数字表面模型(DSM)，它表示地球表面(包括建筑物、基础设施和植被)的高程。COP-DEM是经过编辑的DSM，它来源于WorldDEM产品，编辑包括对水体和不合理地形的处理等。
COP-DEM是当前官方精度最高的开源DEM，绝对高程精度LE90优于4米，绝对平面精度CE90优于6米。
COP-DEM有3种不同的分辨率产品：EEA-10(10米)、GLO-30(30米)和GLO-90(90米)，见图1和图2。EEA-10覆盖39个欧洲国家，陆地覆盖面积600万平方千米；GLO-30和GLO-90覆盖全球，这两个数据集的陆地覆盖面积约为1.49亿平方千米，占地球表面积的29%，见图3。
图1 COP-DEM实例概览(来自哥白尼DEM产品手册)▼
![](https://pic2.zhimg.com/80/v2-ddec7f26c3f5c6523cd928682d4eaf45_1440w.webp)
图2 COP-DEM数据3种空间分辨率对比图(左10m，中30m和右90m) (来自哥白尼DEM产品手册)▼
![](https://pic4.zhimg.com/80/v2-dccaf5c06d785ab697e3640f4fea0a0f_1440w.webp)
图3 COP-DEM(GLO-30和GLO-90)的地表覆盖范围图(来自哥白尼DEM产品手册)▼
![](https://pic3.zhimg.com/80/v2-db6138d3dd8d506e9348b4f2a1a740ea_1440w.webp)
**二、数据源及产品生产**
COP-DEM来源于WorldDEM(见图4)，WorldDEM产品是基于0.4弧秒(对应分辨率10-12米)的TanDEM-X DEM处理后得到的。TanDEM-X DEM由TanDEM-X任务期间获得的全球雷达卫星数据(2010-2015年)经过干涉处理等步骤得到。
图4 COP-DEM来源(来自空客)▼
![](https://pic2.zhimg.com/80/v2-60bd6f27ac6eef37b0945b6369d7d0f1_1440w.webp)
TanDEM-X任务是德国的合成孔径雷达(SAR)全球成像计划，由2颗几乎相同的雷达卫星TerraSAR-X和TanDEM-X组成飞行编队获取全球的X波段干涉数据(见图5)，用于生成全球、均质且高度精确的数字表面模型(DSM)。该任务由代表德国政府的德国宇航中心(DLR)和空中客车防务与航天公司以政府和社会资本合作模式资助。
图5 TerraSAR-X和TanDEM-X卫星组成飞行编队测量地表(来自空客)▼
![](https://pic1.zhimg.com/80/v2-30e374863c9b5df9ff7638535f666078_1440w.webp)
如图6所示WorldDEM进行了需要人工参与的半自动的编辑，经过编辑后的WorldDEM抽样得到30米和90米格网间距的哥白尼DEM(GLO-30和GLO-90)。
图6 从WorldDEM到COP-DEM(来自空客)▼
![](https://pic4.zhimg.com/80/v2-07f8e26821f6f00d4af314236a6768bf_1440w.webp)
WorldDEM的编辑包括地形编辑和水文编辑，具体如下：
**（1）地形编辑**：1）尖峰(spikes)和孔洞(wells)的去除，去除并插值高度差为20m的单个像素；2）空洞(voids)识别和填充，插值的小空隙(最多16像素)，填充了较大的空隙区域；3）噪声编辑，例如平滑阴影区域；4）不真实负高程的升高，海洋沿岸像素升高到0米以上。
**（2）水文编辑**：1）海洋，包括所有海洋、海湾、峡湾均设置为0米；2）湖泊，幅度镶嵌图像中出现的所有内陆水体均设置为单一高程；3）河流，编辑为单调变化的高程。
图7 WorldDEM的水文编辑示例图(来自空客)▼
![](https://pic2.zhimg.com/80/v2-25c6f0d7eae30c380de19743127e9c01_1440w.webp)
**三、数据精度和质量**
哥白尼DEM用户手册中对数据精度的描述见表1，同时表1也包含GLO-30和GLO-90数据集的其它规格参数说明。
表1 Copernicus DEM(GLO-30, GLO-90)规格参数表(DGED和DTED格式)(来自哥白尼DEM用户手册)▼
![](https://pic2.zhimg.com/80/v2-e73f26f488c7c77b28f000f5b1a73259_1440w.webp)
表3-1说明：1）基于TanDEM-X DEM/WorldDEM ICESat GLAS参考点的验证结果(TanDEM-X任务目标：＜10米；全局算术平均值)；2）不包括南极洲和格陵兰岛(在永久性冰雪覆盖的地区，WorldDEM和参考数据的物理反射特性不同)；3）由于TanDEM-X DEM/WorldDEM/Copernicus DEM的全球覆盖范围，本文件中所述的所有精度统计数据和值均作为算术平均值进行计算，可能会出现局部偏差。
哥白尼DEM验证报告文档也给出了数据集的垂直精度验证结果，使用ICESat参考数据进行验证。表2总结了全球精度评估值，约1100万个有效ICESat点，90%(LE90)置信水平下的绝对垂直精度为2.17米，评估结果的平均误差为-1.29米，标准偏差为0.85米。
表2 Copernicus DEM精度结果(来自哥白尼DEM验证报告)▼
![](https://pic2.zhimg.com/80/v2-94110aa6847ceb0d1ab1beb74c1f78c9_1440w.webp)
图8显示了地理单元(1°*1°)验证的绝对垂直精度的空间分布，空白单元格是指ICESat参考点不足的单元格；精度值在2到5米之间的单元格分布在山区以及森林覆盖区，加拿大西海岸由于地形崎岖，精度值较低。
图8 根据统计LE90值分类全球覆盖的地理单元图(来自哥白尼DEM验证报告)▼
![](https://pic4.zhimg.com/80/v2-4dc914a3d8a4595242eb8f1c1eb17b13_1440w.webp)
绝对的水平精度未在验证报告中给出，但是在用户手册中提到绝对水平精度受2个因素影响：(1) 单个DEM景的位置精度，这与TerraSAR-X图像基础产品的精度相关，而其小于0.3米；（2）投影到水平位移的DEM数据的绝对垂直误差。因此绝对水平精度可由绝对垂直误差确定，该绝对垂直误差用LE90ABS<4m的算术平均值表示，则水平精度可确定为圆误差<6m(90%置信水平)。
已有多篇学术论文对哥白尼DEM的精度进行了评估，也与多种开源的DEM进行了对比，例如Li Hui在其论文(参考文献3)中利用ICESat-2测高数据对中国5个区域的Copernicus DEM、NASA DEM和AW3D30 DEM进行了评估，指出对地形表示的视觉检查表明，哥白尼DEM显示了最大的地形细节，其次是AW3D30，然后是NASA DEM。如图9所示，是DEM彩色渲染图和地形剖线图，(a，e)哥白尼DEM，带地形剖面位置指示(蓝线)，(b，f)NASA DEM和(c，g)AW3D30 DEM；还绘制了典型地形剖面(南北)和ICESat-2 GCP用于高程比较(d，h)。地形剖面表明，哥白尼DEM与ICESat-2 GCP最为一致，而AW3D30 DEM总体上高估了高程，NASA DEM总体上低估了高程。
图9 多种DEM (COPDEM - NASADEM -AW3D)目视对比图(来自参考文献3)▼
![](https://pic4.zhimg.com/80/v2-79139564ff0cb1327e34ec0332065267_1440w.webp)
COP-DEM数据还提供额外的质量层信息，质量层是在哥白尼DEM产品生产过程中生成的辅助信息掩膜，是GeoTIFF格式的栅格数据。表3显示了作为哥白尼DEM数据产品一部分的质量层，包括编辑掩膜、填充掩膜、高度误差掩膜、水体掩膜、数据源层、准确度层。图10是编辑数据掩膜示例图。
表3 Copernicus DEM质量层表(来自哥白尼DEM用户手册)▼
![](https://pic2.zhimg.com/80/v2-4be51ec82cf31174e067b746a129d3b1_1440w.webp)
图10 哥白尼DEM彩色渲染图和对应的编辑掩膜示例图(来自哥白尼DEM用户手册)▼
![](https://pic3.zhimg.com/80/v2-7c88aed3706669237b20595cb3a5a152_1440w.webp)
**四、数据访问和下载**
全球COP-DEM数据下载不限于以下3种方式：
（1）欧空局哥白尼panda网站：[https://panda.copernicus.eu/panda](https://link.zhihu.com/?target=https%3A//panda.copernicus.eu/panda)
（2）OpenTopography网站：[https://portal.opentopography.org/datasetMetadata?otCollectionID=OT.032021.4326.1](https://link.zhihu.com/?target=https%3A//portal.opentopography.org/datasetMetadata%3FotCollectionID%3DOT.032021.4326.1)
（3）QGIS下载：安装OpenTopography DEM Downloader插件。
最后把之前分享过的哥白尼DEM(30米)中国区域分块镶嵌数据再发一遍，之前的链接有效期过了，下载链接(有效期到20231020)：[https://pan.baidu.com/s/1BOIRzvffuOcxqpDikPlPUw](https://link.zhihu.com/?target=https%3A//pan.baidu.com/s/1BOIRzvffuOcxqpDikPlPUw) 提取码：diy2
图11 COP-DEM GLO30中国区域分块镶嵌数据示意图▼
![](https://pic3.zhimg.com/80/v2-514c325aa59506b71747745f44f4ab02_1440w.webp)
感谢阅读，如有任何问题和建议请发私信或联系我！欢迎关注并星标“石头人看遥感”（宫浩，你懂得），并转发让更多的人看到。您的每一次点赞、转发，都是对我的肯定和支持，谢谢！
**参考文献**
_[1] Copernicus DEM Product Handbook, June 2022.[2] Copernicus DEM Validation report, Nov 2020.[3]Li Y Y, Li L Y, Chen C F, et al. Correction of global digital elevation models in forested areas using an artificial neural network-based method with the consideration of spatial autocorrelation. International Journal of Digital Earth, 2023,16(1): 1568-1588._