---
{"title":"Rhino_练习","tags":["software"],"dg-publish":true,"dg-note-icon":"2","dg-path":"⚒️ Software/Rhinoceros 3D/Rhino_Practice.md","permalink":"/⚒️ Software/Rhinoceros 3D/Rhino_Practice/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-05T23:48:02.949+08:00"}
---

-   Bosjes 教堂 / Steyn Studio![](https://api2.mubu.com/v3/document_image/a7e49bd3-0fce-4687-abe1-7a6acfc99cb7-20454557.jpg)  
    floating in the surrounding nature  
    [Bosjes 教堂 / Steyn Studio | ArchDaily](https://www.archdaily.cn/cn/867611/bosjes-jiao-tang-steyn-studio?ad_source=search&ad_medium=projects_tab)建筑师: [Steyn Studio](https://www.archdaily.cn/cn/office/steyn-studio?ad_name=project-specs&ad_medium=single)面积 : [430](https://www.archdaily.cn/search/cn/projects/min_area/344/max_area/516?ad_name=project-specs&ad_medium=single) m²  
    项目年份 : [2016](https://www.archdaily.cn/search/cn/projects/year/2016?ad_name=project-specs&ad_medium=single)  
    地址: 99 Voortrekker St, Ceres, 6835, South Africa  
    新教堂位于南非葡萄园内，由伦敦 Steyn 工作室的 Coetzee Steyn （出生在南非）设计。它以周边山脉的轮廓为出发点，呼应 Western Cape 村庄的历史古迹 Cape Dutch 的三角墙。屋顶由一个纤薄混凝土的外壳构成，独自承重，每个波形轮廓正好连着地面。在每个波浪型屋顶的顶端，窗口的中央连着十字架装饰的外墙。  
    -   1.对照原有平面图用矩形线描出轮廓，再用「PlanarSrf」 以平面曲线建立曲面封面  
    -   2.对该曲面进行「Rebuild」重建曲面，设置U方向10个点、V方向6个点、3阶。拖动相应的控制点做造型。  
    -   3.将两侧最外侧的控制点全选，右键「Rotate」 旋转向内进行3D旋转12°。![](https://api2.mubu.com/v3/document_image/57f65da6-f0a7-422d-a6e6-fb2ae1e12d4a-20454557.jpg)  
    -   4.将曲面「DupBorder」复制边框后用「ExtendSrf」延伸曲面将曲面的四个边进行延伸一部分，类型直线。![](https://api2.mubu.com/v3/document_image/37b2096a-bce6-4e0c-8842-f011e06780e1-20454557.jpg)  
    -   5.整体向内「OffsetSrf」偏移曲面一个合适的厚度  
    -   6.将复制的边框沿着Z方向复制一份并「SetPt」设置XYZ坐标，向下「ExtrudeCrv」直线挤出贯穿多重曲面。![](https://api2.mubu.com/v3/document_image/f9fbd87a-74e2-4adf-9d67-3e4391a64f83-20454557.jpg)  
    -   7.利用挤出物件将延伸出去的多重曲面边缘「Trim」修剪。再利用多重曲面将多余的挤出物件修剪。  
    -   8.用线将多重曲面分割为4等份，取其1  
    -   9.将边缘向下「Offset」偏移，与工作平面平行选否。然后在将其刚才的边缘「Loft」 放样，用得到的面对原有多重曲面进行修剪。![](https://api2.mubu.com/v3/document_image/bbd702db-2c29-4f58-a4e2-0ff9b83e57de-20454557.jpg)  
    -   10.将多重曲面「Explode」 炸开，选择最下面的曲面「Isolate」隔离物件，并用线将需要加厚的地方进行分割。![](https://api2.mubu.com/v3/document_image/1b10655f-6fec-40d0-a124-c6d36f8e744d-20454557.jpg)  
    -   11.将曲面「DupEdge」复制边缘后删除。  
    -   12.将复制的边缘进行「FitCrv」以公差重新逼近曲线，公差0.1。并将最下面的控制点向下拖动到合适的位置。注意拖动控制点时要用「CPlane」设置工作平面至物件保证在对应侧面的工作平面上拖动。![](https://api2.mubu.com/v3/document_image/b5101a37-b288-49df-a671-4b0528a814bf-20454557.jpg)  
    -   13.缺口的三个边缘，和刚逼近的曲面一起用「NetworkSrf」从网线建立曲面封面。并用OD显示模式检查曲面顺滑度，如需调整可用「MatchSrf」衔接曲面进行衔接，先保证连续性然后在精准衔接。![](https://api2.mubu.com/v3/document_image/6e418bc3-aaa8-416a-b69d-e6349f88a477-20454557.jpg)![](https://api2.mubu.com/v3/document_image/847b582a-9bdd-4754-8ff6-9c0b7540e7f2-20454557.jpg)  
    -   14.取消隐藏，在缺口边缘处画垂直线到侧面上，修剪多余的面。![](https://api2.mubu.com/v3/document_image/18f91d31-0365-47fb-a4a0-7b70a2ab5e05-20454557.jpg)  
    -   15.用「CurveBoolean」曲线布尔运算将剩下的面补全，在进行「Mirror」 镜像将其余面补全。![](https://api2.mubu.com/v3/document_image/b1360b67-b08f-4317-a262-41662e324574-20454557.jpg)  
    -   16.深化一下玻璃幕墙以及十字架等细节。![](https://api2.mubu.com/v3/document_image/f00d1c59-2d34-49ad-9ff2-0d67219e756f-20454557.jpg)  
-   金属彩虹里的书店-苏州钟书阁 / Wutopia Lab![](https://api2.mubu.com/v3/document_image/e9afdcb1-9812-420d-abe1-ae6206359b07-20454557.jpg)  
    [金属彩虹里的书店-苏州钟书阁 / Wutopia Lab | ArchDaily](https://www.archdaily.cn/cn/877844/jin-shu-cai-hong-li-de-shu-dian-su-zhou-zhong-shu-ge-wutopia-lab?ad_source=search&ad_medium=projects_tab)建筑师: [Wutopia Lab](https://www.archdaily.cn/cn/office/wutopia-lab?ad_name=project-specs&ad_medium=single); Wutopia Lab  
    面积 : [1380](https://www.archdaily.cn/search/cn/projects/min_area/1104/max_area/1656?ad_name=project-specs&ad_medium=single) m²  
    项目年份 : [2017](https://www.archdaily.cn/search/cn/projects/year/2017?ad_name=project-specs&ad_medium=single)  
    地址 : 苏州市,中国
    -   1.载入项目平面图![](https://api2.mubu.com/v3/document_image/9f97cff8-dd5a-403a-ae61-a20bce81430b-20454557.jpg)  
    -   2.细分出大体快![](https://api2.mubu.com/v3/document_image/7462f02e-f380-4759-9816-e44bc87ad382-20454557.jpg)  
    -   3.手工调整SubD造型![](https://api2.mubu.com/v3/document_image/ad258f7b-f668-44fd-b799-85788f198a1b-20454557.jpg)  
    -   4.拾取进Grasshopper,并转为Brep  
    -   5.给该物件做厚度,提取「BoundingBox」边框方块的顶点,向上移动,提取Brep的边线并简化,通过「Shatter」分割曲线打断并提取点的z轴高度,筛选出小于2.5米的直线,这会影响后期的成面。![](https://api2.mubu.com/v3/document_image/7a4c9963-5b75-41aa-9902-424056b1c776-20454557.jpg)  
    -   6.将这些线用「Loft」放样曲面成面并拍平，并封顶，和之前的Brep一起用「Brep Join」曲面组合组合成一个Brep。![](https://api2.mubu.com/v3/document_image/4a3a3b59-1b5e-48f2-8939-b6b234155721-20454557.jpg)  
    -   7.通过打断后的线组合，用「Discontinuity」提取曲线拐角点（或其他连续性级别的点）打断刚组合的线筛选出切片的基础线。![](https://api2.mubu.com/v3/document_image/f436e1f5-e84a-4d36-996a-9a5be5ddb6c0-20454557.jpg)  
    -   8.用基础线等分并求点到偏移后的线最近点得到两个点并连线。然后再延伸出Brep的范围。![](https://api2.mubu.com/v3/document_image/abe989ad-18e6-4080-9400-f2dbb1ac6168-20454557.jpg)  
    -   9.将线投影至Brep上，并封面，再通过「Gradient」色彩渐变器给颜色。![](https://api2.mubu.com/v3/document_image/c1abc2c4-978e-4122-a906-71af0eed36e0-20454557.jpg)  
-   成都独角兽 /Zaha Hadid Architects![](https://api2.mubu.com/v3/document_image/489202a7-73fa-46fa-872c-58ccef87b730-20454557.jpg)  
    [成都独角兽岛总体规划首座建筑即将完工 / Zaha Hadid Architects - 谷德设计网 (gooood.cn)](https://www.gooood.cn/unicorn-island-masterplan-first-building-nears-completion-zaha-hadid-architects.htm)  
    设计公司:[Zaha Hadid Architects](https://www.gooood.cn/company/zaha-hadid-architects)位置 : 成都  
    类型 : [建筑](https://www.gooood.cn/category/type/architecture)  
    -   1.画出基准线。![](https://api2.mubu.com/v3/document_image/ca450b5e-2c79-4280-8263-6cc00ea5bcc7-20454557.jpg)  
    -   2.「Loft」 放样成面。![](https://api2.mubu.com/v3/document_image/ff68dfb7-de2c-4a1d-818a-8e8e0bc63e91-20454557.jpg)  
    -   3.载入Grasshopper，提取结构线将其分为两组。  
    -   4.先处理玻璃部分，通过LunchBox里的Triangle Panels B将面 细分为三角形表皮，再利用高度值将其排序，打乱顺序并分组。![](https://api2.mubu.com/v3/document_image/999b397b-b2f2-483a-9e02-a1b509d7aba2-20454557.jpg)  
    -   5.接下来处理开洞玻璃部分，将另一组利用中心点到外侧边缘得距离排序并分组，然后进行随机打乱得到开洞得玻璃面，在进行偏移成面。![](https://api2.mubu.com/v3/document_image/814f5e76-16cd-48d0-94a4-277eeae606b9-20454557.jpg)  
    -   6.其余部分取其侧面得结构线，进行等分并投影到曲面上成结构线，并切割。![](https://api2.mubu.com/v3/document_image/d0a030b0-a6e1-46bb-be74-f6f6cef3ccc2-20454557.jpg)  
    -   7.最后Bake后赋予材质![](https://api2.mubu.com/v3/document_image/f4cf57e6-1ded-4bcd-b6af-e208c204d9c2-20454557.jpg)