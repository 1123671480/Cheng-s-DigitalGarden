---
{"tags":["software"],"type":["渲染器"],"dg-publish":true,"dg-note-icon":"2","dg-path":"Software/Render/D5_Render For Rhino.md","permalink":"/Software/Render/D5_Render For Rhino/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-10-09T09:33:06.000+08:00","updated":"2024-11-05T23:48:02.962+08:00"}
---

# 简介  
-   D5渲染器是一款国产的实时渲染器，拥有非常强大的RTX光线追踪技术和光栅化两种渲染方式，支持HDR照明，常用于室内等。同时可以联动SketchUp、[[D 📚 RESOURCE/⚒️ Software/Rhinoceros 3D/Rhino\|Rhino]]等等，做到同步预览。  
# 视角  
-   分两种，一种和Lumion一样「WASD」移动「右键」旋转视角「QE」升降，还有一种是固定主体物旋转相机，类似SketchUp  
# 常规工作流  
-   检查模型  
	-   是否有法线面的正反问题  
	-   材质UV调整问题  
	-   模型是否有破面  
-   Rhino联动  
-   设置相机  
-   调整自然光 人工光  
-   调整材质  
-   后期  
# 自然光照  
-   室内场景  
	-   要给相机后方留有空间  
	-   外墙必须为双面墙体  
-   调整相机设置场景号  
-   「太阳」亮度不要太高角度高度根据需要调整  
-   「阴影半径」是控制阴影的虚实  
-   可以贴HDR天空，不过无法调整大高度  
# 人工光照  
-   「1」点光源  
-   「2」聚光灯  
-   「3」灯带  
-   「4」区域光  
-   材质自发光给0.1  
-   按住「Shift」、「Ctrl+D」可以复制光源  
# [[D 📚 RESOURCE/⚒️ Software/Render/Physicallly_Based Rendering\|Physicallly_Based Rendering]]（PBR）
-   「PBR」名词讲解 基于物理的渲染技术背景下的金属度粗糙度材质描述体系  
-   金属度  
	-   材质是否为金属，是调1，否调0 铁锈金属度0  
-   高光-非金属反射层强弱  
	-   默认0.5 玻璃为0.5 水为0.25 玉石为1  
-   粗糙度  
	-   大多数材质粗糙度为0.2以内  
-   镜子  
	-   金属度1 粗糙度0 反射白色  
	-   SketchUp材质导入自动为粗糙无反射的非金属材质  
	-   法线贴图可以给材质一种真实的凹凸强度  
	-   「Color」「Base Color」「Albedo」「Diffuse」为材质底色  
	-   「Metallic」「Metalness」为金属贴图  
	-   「Normal」为法线信息 紫色图  
	-   「Specular」为高光 用于描述反射层的强度 灰度图  
	-   「Glossiness」反色可以得到「Specular」  
-   制作金属铁锈贴图  
	-   用Photoshop打开金属贴图-「去色」-「Ctrl+L」调高对比度  
# 后期出图  
-   D5有一套完整的后期调色参数  
-   「F8」两点透视  
-   可同时导出通道图5