---
{"dg-publish":true,"permalink":"/🍊 TANGERINE/Obsidian/Obsidian/","tags":["software"],"noteIcon":"1","created":"2024-09-24T22:57:38.000+08:00","updated":"2024-11-28T23:16:14.626+08:00"}
---

## Obsidian 是什么

是一款本地的、扩展性极强的、使用 Markdown 纯文本格式的、支持双链的适用于构筑 [[🍊 TANGERINE/Nexp/PKM\|PKM]] 知识管理第二大脑的笔记软件。借用官网的话来说：

> Obsidian is a **powerful and extensible** knowledge base that works on top of your **local folder** of **plain text files**.
“Obsidian 是一个强大且扩展性极高的知识库，建立在你本地文件夹中的纯文本文件中。”——摘自[Obsidian 官方网站](https://obsidian.md/)

### Obsidian 的优势

由于 Obsidian 是基于 Markdwon 纯文本的，一切都尊重纯文本来构建的，最大的好处是脱离 Obsidian 也可读。这就导致有上手难度，但对于大多数人来说，几乎很快就能适应，操作习惯可以通过社区插件弥补。主要难点就只有 Markdown 语法，这种语法格式在知乎，简书，Github 等各大平台都支持，是一种非常优雅的写作方案。

Obsidian 的优点集中在：

- **知识管理**：不单单是文字编辑器，和 word，vim 这些有本质上的区别。学习 ob 的目的不仅仅是为了记笔记，而更多的是打造自己的**知识体系**，Obsidian 提供笔记管理的工具罢了。这些工具包括但不限于：
	- 优化输入体验（vim 模式，模板，自动补全，代码高亮，智能列表，折叠缩进，智能粘贴，图片、音频、视频、网页等多媒体插入）
	- 笔记关联（双链，标签，块引用，关系图谱）其中双链笔记实组织 [[🍊 TANGERINE/Nexp/PKM\|PKM]] 知识管理、第二大脑的必备方式
	- 高度开放的插件系统。
- **本地化**：Obsidian 不依赖于网络就可以正常运行，所有的数据都保存到本地，数据永远在自己手里。Obsidian 管理的所有数据都存在于一个文件夹中，这个文件夹称之为库 ([[🍊 TANGERINE/Nexp/Vault\|Vault]])，包括配置文件和笔记文件。其中配置文件以 `.obsidian` 存在于库的根目录中，管理着 ob 的主题，样式，插件和一些运行时的数据。这带来了易于迁移和同步的特性。
- **扩展性高**，**社区生态活跃**：每个人不仅可以定制独特的外观，还可以自动化自己的工作流。无代码能力的可以享受社区带来的种种惊喜。正是因为每个人做知识管理的目的和习惯都不同，高度自定义才能满足绝大部分人的需要。所谓的生态主要集中在两个方面，一方面是用 Obsidian 的分享，另一方面是 Obsidian 主题和插件。目前社区里有近 2000+ 各式各样的插件，185+ 主题，同时有大量的其他插件主题未上架。论坛有超过 20000+ 帖子 (除去 bug 反馈)，知乎，B 站等地分布着各式各样的教程和分享，仅 Discord 就有接近 10 万人。
- **纯文本格式**：以 [[🍊 TANGERINE/Nexp/Markdown\|Markdown]] 格式为基础的储存格式，文件架结构透明，可以随时转移不受限制，占地 空间小，这意味着即使脱离 Obsidian 软件，也是肉眼可读的，借助一些 [[🍊 TANGERINE/Nexp/Markdown\|Markdown]] 编辑器，也有不错的体验。
### Obsidian 生态

- Dataview 插件 
- Tasks + Templater 插件使我构筑好个人 [[🍊 TANGERINE/Nexp/GTD\|GTD]] 系统
- Quickadd 插件使我完成了库内大部分的自动化，如一键录入灵感、建立 Tasks 、快速新建模板笔记等等
- Map View 插件使我完成了个人 GIS 系统，可以标记自己去过/想去的地点、做旅游攻略等
- Vran 大佬开发的 Components 插件 几乎实现了 Notion database 80%的功能，为 [[🍊 TANGERINE/Obsidian/Cheng\|Cheng]] 的核心之一
- 详情另见 [[🍊 TANGERINE/Obsidian/Community Plugins\|Community Plugins]]

Obsidian 的生态主要围绕着 Discord 和 [英文社区](https://forum.obsidian.md/) 展开的，这是因为两位创始人生活在加拿大，自然而然主要用户集中在欧美国家。据 [OSS Insight](https://ossinsight.io/) 统计，国内用户占到 25% 左右。国内社区的运营分散在互联网的各个角落，前期主要是以个人分享的内容为主，比如 [Ryooo](https://www.zhihu.com/people/rao-yao-47-68)，[Boninall](https://www.zhihu.com/people/kio-mis) 等人，大多是为爱发电，所以不温不火的。

这就导致了 Obsidian 的内容多以英文为主，对许多人来说有着不小的门槛。唯一能解决的就是建立国内的软件生态，Pkmer 倒是有意接过这杆大旗。

在 2020 年诞生的 Obsidian，至今都是凭借着创始人和社区贡献者的热情和奉献勇往直前的，开发团队都来自使用和开发 Obsidian 插件的社区人员。综上所述，Obsidian 是一个值得信任的笔记软件。

## Obsidian 开发团队

目前的开发者有八位，前两位是 Obsidian 的创始人，分别是：

- Shida Li：负责后端，之前在 Dropbox 和 Linkedin 工作，滑铁卢大学 17‘ 软件工程专业
- Erica Xu：负责前端和 UI，之前在 Quizlet 工作，滑铁卢大学 16’计算机科学专业
- Stephan Ango：Obsidian 的 CEO，是 Minimal 主题，Hider 插件，System Dark Mode 的开发者
- Liam Cain：负责编写代码并审查新的社区插件，在加入 Obsidian 之前，是 Calendar，Periodic Notes，Creases，Lapel，Things Logbook 插件的开发者
- Mattehew Meyers：前软件工程师，目前是位医生。是 Kanban，Style Settings，Pandoc Reference List 等十几个优秀插件的开发者。
- Sandy：办公室一号喵，轻音体柔喵喵叫。
- Blaze：办公室二号喵，像狗一样贼有活力，爱玩捉迷藏，更爱摇尾巴。

## Obsidian 付费问题

|     | 个人                                 | 赞助者               | 商业使用               |
| --- | ---------------------------------- | ----------------- | ------------------ |
| 权益  | 个人 **完全免费**，无需登录，可访问所有插件和 API，社区支持 | 支持开发，内测，社区徽章，开发频道 | 14 天免费试用，商业使用，优先支持 |
| 价格  | **$0**                             | 一次性赞助 **$25** 以上  | 每个用户每年 **$50**     |

另外一个收费项目是增值服务：

|        | 同步                                                                                                                       | 发布                                                                                                                                             |
| ------ | ------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| 权益     | 端到端加密，版本历史，邮件优先支持                                                                                                        | 零门槛需求，笔记选择性发布，关系图和大纲，邮件优先支持                                                                                                                    |
| 价格     | 年付 $8/月                                                                                                                  | 年付 $16/月/站点                                                                                                                                    |
| 个人解决办法 | 第三方同步也不稳定冲突，iCloud 同步也经常冲突，百度云同步盘不支持带有 emoji 的文件。最后还是选择了官方同步，淘宝拼车 118 一年，是真香，好用是真的好用，达到类似幕布的无感同步，还特别稳不会冲突，详见 [[🍊 TANGERINE/Obsidian/Sync\|Sync]] | 为建立数字花园我采用了 Obsidian-Digital-Gander 插件作为搭建桥梁，以 [Netlify](https://app.netlify.com) 作为构筑网站，以 Gtihub 作为代码托管。最终发布了🍊橘园，详见 [[🍊 TANGERINE/Garden Management/Construction Process\|Construction Process]] |

是否会在未来收费这也是一个很大的问题，我个人倾向于这个免费 Obsidian 本体应该是永久的，基于下面的考虑：

1. 不管是在 Discord 上的 Shida Li 还是 Reddit 上的 Obsidian CEO Stephan Ango 都曾说过，Obsidian 都不会商业化运营，即不会拉投资，使得这款软件以盈利为主要目的。前者发生在与 Heptabase 的聊天中，后者发生在 Stephan Ango 成为 Obsidian CEO 在 Reddit 上的问答，很有参考价值。
2. 如果 Obsidian 的本体收费，这将把 Obsidian 的插件开发者置于一个很尴尬的境地，不知道如何处理
3. Obsidian 是本地笔记软件，可全程不联网不注册，即使收费了也可无压力使用。得益于本地 Markdown 格式，迁移非常方便。
4. 即使开源，收不收费依旧由开发者决定。可以参考 [Auto.js](https://github.com/clearw5/Auto.js) 在开源后有着一万两千 star 后选择闭源收费。

所以 **关心是否永久免费是没必要的**，一方面开发者承诺终生使用是不负责的可行性也极低，另一方面我们是否会在将来迁移到更好的笔记软件也是未可知的。

## Obsidian 的使用

对于 Obsidian 新手用户，请先参看 [[Obsidian新手指南\|Obsidian新手指南]]。

### 目录概述

Obsidian 的使用需要清楚 [^1] 三个目录：

1. 软件安装目录：从官网下载安装后自动创建的 ，`C:\Users\<用户名>\AppData\Local\Obsidian` ，这个目录是软件运行的必须文件，最好不要做任何修改。
2. 软件缓存目录：同样是安装后自动创建的，Windows 电脑在 `C:\Users\<用户名>\AppData\Roaming\obsidian`，这个目录保存着软件索引缓存，全部库的地址缓存，快照，沙盒库等，最好不要做任何修改。
3. 库目录：这在打开 Obsidian 时，会让你选择一个文件夹，该文件夹将存放所有的个人数据，包括 Obsidian 的配置，插件，主题，笔记等

其中着重注意库目录，这个文件夹包含了你整个个人数据，备份这个文件夹，你将可以在任何能安装 Obsidian 的地方还原包括笔记，插件，主题，快捷键，布局等在内的所有配置。它长这样

```
Pkmer-Docs
├── .obsidian   //obsidian的配置文件夹
├── 00-关于
├── 01-社区资源合集
├── 02-知识管理基础
├── 03-知识管理工具
├── 10-Obsidian
├── 20-深入理解知识管理
├── 30-知识管理应用
├── 40-开发者指南
├── 90-其它
├── Config
├── License
├── README.md
├── Resource
└── 主页.md
```

除了默认的 `.obsidian` 外，其余的都是你的笔记。这个文件夹各部分如下：

```
.obsidian
├── app.json  //整个软件的配置
├── appearance.json  //外观配置
├── bookmarks.json   //bookmarks核心插件的配置
├── canvas.json      //白板canvas的配置
├── community-plugins.json    //社区插件列表
├── core-plugins-migration.json  //核心插件配置
├── core-plugins.json  //核心插件配置
├── graph.json  //图谱配置
├── hotkeys.json  //快捷键配置
├── plugins  //插件目录，所有安装的第三方插件都在这，手动安装的基础
├── themes   //主题目录，所有安装的第三方主题都在这，手动安装的基础
└── workspace.json  //工作区配置
```

这些配置都是自动生成的，无需担心，一般仅在第三方插件或主题出问题时才会有需要操作其中的 `plugins` 和 `themes` 文件夹。

[^1]: 知道这些可以理解一些高级操作，比如所有库通过符号链接共用一个配置，脚本修改库的地址缓存实现更改打开的默认库等