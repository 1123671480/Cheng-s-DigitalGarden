---
{"dg-publish":true,"permalink":"/C 📔 AREA/🖥 Equipment/System/MacOS/","title":"MacOS","noteIcon":"1","created":"2025-08-16T13:55:24.215+08:00","updated":"2024-12-28T13:46:25.723+08:00"}
---

-   MacOS的大脑![](https://api2.mubu.com/v3/document_image/52e7d0b6-3705-4c66-bb3a-4e313781b881-20454557.jpg)  

## 删除文件

-   `·sudo rm -r -f` 要删除的文件  

## 显卡模式

-   `sudo pmset -a GPUSwitch 0`
	-   0-强制使用核显 
	-   1-强制使用独显  
	-   2-自动切换显卡  

## Mac经典开机启动音

-   ```sudo nvram StartupMute=%00`  
	-   00-开启  
	-   01-关闭

## 修改文件创建时间/修改时间


修改文件创建时间`set file -d ‘mm/dd/yy hh:mm:ss’ filename`
修改文件修改时间`set file -m ‘mm/dd/yy hh:mm:ss’ filename`