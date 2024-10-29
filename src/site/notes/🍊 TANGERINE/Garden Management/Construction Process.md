---
{"dg-publish":true,"dg-note-icon":2,"author":["橘子"],"dg-path":"Garden Management/Construction Process.md","permalink":"/Garden Management/Construction Process/","dgPassFrontmatter":true,"noteIcon":2,"created":"2024-10-26T20:16:51.000+08:00","updated":"2024-10-29T23:52:34.979+08:00"}
---

### Construction
- 这里只叙述搭建思路，不详说搭建步骤
- 数字花园是基于Obsidian的，所以搭建基础是一个Obsidian的Vault，我们的所有发布内容都写在Vault中，过第三方插件Obsidian-Digital-Gander进行发布，根据[Obsidian-Digital-Gander官方说明](https://dg-docs.ole.dev/)的指引，您先需要在GitHub注册账号并且指定一个仓库进行网站代码托管，并以[Netlify](https://app.netlify.com)作为构筑网站，免费用户可以有100GB的流量以及300分钟的构筑时间。
- 前期构筑完成后，您将拥有一个初始界面，可以在Obsidian中把需要发布的笔记的元数据（frontmatter）加上`dg-publish：true`
- 您需要定义一篇笔记作为网站的主页，请在元数据加上`dg-home: ture`
- 这样再运行Obsidian-Digital-Gander的命令Publish Center（发布中心），选择要发布/修改/删除的笔记后点击PUBLISH SELECTED，等待一段时间就可以在您的数字花园中看到已发布的笔记

>您可以打开[Netlify](https://app.netlify.com)查看实时构筑情况，有时会出现各种意外情况导致构筑失败，请回想起是不是哪些元数据拼写错误，也可以点击构筑网站内的AI总结错误原因，最后可以看一下构筑日志中报错的部分

- 网站构建对于新手来说比较困难，不过构筑成功后非常有成就感！橘子也一直在摸索中……
### Log
- 2024-10-26：初步搭建Digital Garden，更名为🍊Tangerine|橘园
- 2024-10-28：添加主页Tree Graph，并且绘制了主页Icon
- 2024-10-28：【构筑问题】原因：笔记元数据中的Icon格式问题，只能是“1、2、3、withered、stone、signpost”
- 2024-10-29：更改CSS设置，更改主页Icon为🍊
- 2024-10-29：【构筑问题】原因：网站图标必须是正方形