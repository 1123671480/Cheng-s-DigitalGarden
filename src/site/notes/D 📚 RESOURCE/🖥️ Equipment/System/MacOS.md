---
{"title":"MacOS","dg-publish":true,"dg-note-icon":"1","dg-path":"🖥️ Equipment/System/MacOS.md","permalink":"/🖥️ Equipment/System/MacOS/","dgPassFrontmatter":true,"noteIcon":"1","created":"2024-07-04T13:45:17.000+08:00","updated":"2024-11-05T23:48:02.936+08:00"}
---

-   MacOS的大脑![](https://api2.mubu.com/v3/document_image/52e7d0b6-3705-4c66-bb3a-4e313781b881-20454557.jpg)  

# 删除文件  

-   `·sudo rm -r -f` 要删除的文件  

# 显卡模式  

-   `sudo pmset -a GPUSwitch 0`
	-   0-强制使用核显 
	-   1-强制使用独显  
	-   2-自动切换显卡  

# Mac经典开机启动音  

-   ```sudo nvram StartupMute=%00`  
	-   00-开启  
	-   01-关闭

