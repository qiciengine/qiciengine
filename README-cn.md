<p align="center"><a href="http://www.zuoyouxi.com" target="_blank"><img src="images/logo.png"></a></p>

# 青瓷引擎

- [介绍](#介绍)
- [技术堆栈](#技术堆栈)
- [功能特点](#功能特点)
- [入门](#入门)
- [文档](#文档)
- [例子](#例子)
- [参与](#参与)
- [变更记录](#变更记录)
- [联系我们](#联系我们)
- [授权协议](#授权协议)

## 介绍

青瓷引擎是一款开源免费的 JavaScript 游戏引擎类库，并提供了一站式基于浏览器的 HTML5 游戏开发工具套件。

采用青瓷引擎，开发 HTML5 游戏和传统 Web 网页开发一样，使用任何你喜欢的编辑器，使用任何你喜欢的浏览器，利用 JavaScript 语言和所有先进的 Web 开发工具，让青瓷引擎处理底层技术的复杂性，你只需要关注最重要的事情：做游戏！

<img width='400' src="images/overview.png">

## 技术堆栈

青瓷引擎基于开源免费得 HTML5 游戏框架 [Phaser](http://phaser.io/)，其采用 [Pixi.js](http://www.pixijs.com/) 作为底层渲染引擎，实现 WebGL 和 Canvas 两种渲染模式的跨桌面和移动终端浏览器支持。

Phaser 主要由 [@photonstorm](https://twitter.com/photonstorm) 持续的开发和维护发展，青瓷引擎基于的是 Phaser 2.3.0 版，但我们持续的跟踪关注的 Phaser 的任何版本改动升级，任何 bug 修复和性能提升我们都会整合到青瓷引擎中，因此用户尽管放心使用青瓷引擎发布包中所带的 Phaser 版本即可。

青瓷引擎由三部分组成：QICI Core、QICI Widget 和 QICI Editor

QICI Core：一套基于 Phaser 的 JavaScript 游戏引擎类库。  
QICI Widget：一套 JavaScript 通用图形组件库。  
QICI Editor：一套基于浏览器的跨平台集成式游戏编辑器，包含基于 [Node.js](http://nodejs.org/) 的后台服务。  

QICI Core 是青瓷引擎的核心模块，QICI Editor 需要基于 QICI Core 才可运行，但 QICI Core 无需 QICI Editor 也可独立工作，通过编程创建 HTML5 游戏。但没有 QICI Editor 这种所见即所得的功能支持，很难维护和构建用户界面稍微复杂点的游戏，采用 QICI Editor 甚至可以让美工和策划参与帮助构建用户游戏界面。

QICI Widget 提供了一整套构建 QICI Editor 所需的基于 HTML5 的 UI 通用组件库

QICI Core 是基于 JavaScript 的游戏引擎类库，QICI Widget 是基于 JavaScript 的图形组件类库，QICI Editor 采用 Node.js 进行本地文件系统资源操作，因此可以说青瓷引擎是全栈 JavaScript 的游戏引擎。

<img width='400' src="images/techstack.png">

## 功能特点

- **QICI Core**
    - WebGL 和 Canvas 渲染支持
    - [界面组件](http://docs.zuoyouxi.com/manual/UI/Sample.html)：开关、拉条、进度条、滚动视图、列表等等
    - [界面布局](http://docs.zuoyouxi.com/manual/UI/BasicLayout.html)
    - [骨骼动画](http://docs.zuoyouxi.com/manual/DragonBone/index.html)
    - [九宫格](http://docs.zuoyouxi.com/manual/NinePatch/index.html)
    - [节点遮罩](http://docs.zuoyouxi.com/manual/BuildinComponents/NodeMask.html)和[着色器](http://docs.zuoyouxi.com/manual/Filter/index.html)效果
    - 混合 [Dom](http://docs.zuoyouxi.com/manual/Sample/Dom.html) 和 Canvas 功能
    - [网页字体](http://docs.zuoyouxi.com/manual/WebFont/index.html)和[图片字体](http://docs.zuoyouxi.com/manual/BitmapFont/index.html)
    - [瓦片地图](http://docs.zuoyouxi.com/manual/Sample/Tilemap.html)
    - [Web Audio 和 Audio Tag](http://docs.zuoyouxi.com/manual/Sound/index.html)
    - [Tween 动画](http://docs.zuoyouxi.com/manual/Tween/index.html)
    - [面向组件脚本架构](http://docs.zuoyouxi.com/manual/Behaviour/index.html)
    - [资源管理](http://docs.zuoyouxi.com/manual/AssetsLoad/index.html)
    - 场景和预制[序列化](http://docs.zuoyouxi.com/manual/Serializer/index.html)
    - 鼠标、键盘和触摸支持
    - [Excel 数据导入](http://docs.zuoyouxi.com/manual/Excel/index.html)
    - 插件系统如内置的[物理](http://docs.zuoyouxi.com/manual/Plugin/Arcade.html)和[锁屏](http://docs.zuoyouxi.com/manual/Plugin/LockOrientation.html)等插件
- **QICI Editor**
	- [工程管理](http://docs.zuoyouxi.com/manual/Project/index.html)
	- [场景管理](http://docs.zuoyouxi.com/manual/Scene/index.html)	
	- [层次面板](http://docs.zuoyouxi.com/manual/Interface/Hierarchy.html), [游戏面板](http://docs.zuoyouxi.com/manual/Interface/Scene.html)和[监视面板](http://docs.zuoyouxi.com/manual/Interface/Inspector.html)
	- [图集打包](http://docs.zuoyouxi.com/manual/Atlas/index.html)
    - [帧动画编辑](http://docs.zuoyouxi.com/manual/FrameAnimation/index.html) 
	- [曲线动画编辑](http://docs.zuoyouxi.com/manual/Tween/index.html)
	- [九宫格编辑](http://docs.zuoyouxi.com/manual/NinePatch/index.html)
	- [骨骼动画导入和预览](http://docs.zuoyouxi.com/manual/DragonBone/index.html)
	- [编辑器扩展](http://docs.zuoyouxi.com/manual/ExtendEditor/index.html)
	- [工程设置](http://docs.zuoyouxi.com/manual/Settings/index.html)
	- [工程发布](http://docs.zuoyouxi.com/manual/Publish/index.html)

你甚至可以在移动终端浏览器打开 QICI Editor 进行游戏开发：  
<img width='400' src="images/iphone.jpg"><br><img width='400' src="images/dota.png"><br><img width='400' src="images/ipad.jpg">

## 入门

- 根据[安装手册](http://docs.zuoyouxi.com/manual/Overview/Install.html)安装 [Node.js](http://nodejs.org/)，[下载最新版](http://bbs.zuoyouxi.com/forum.php?mod=viewthread&tid=86&page=1&extra=#pid103)的青瓷引擎。
- 阅读[工程管理手册](http://docs.zuoyouxi.com/manual/Project/index.html)创建一个新工程。
- 阅读[场景编辑手册](http://docs.zuoyouxi.com/manual/Scene/index.html)创建一个新场景。
- 阅读[界面组件手册](http://docs.zuoyouxi.com/manual/UI/index.html)添加些组件到界面场景。
- 从[工具条](http://docs.zuoyouxi.com/manual/Interface/ToolBar.html)点击"运行"按钮，或从[主菜单](http://docs.zuoyouxi.com/manual/Interface/MainMenu.html)选择"编辑/预览(WebGL)"进行游戏运行和测试。

## 文档

官网的文档分为以下几部分：

- [使用手册](http://docs.zuoyouxi.com/manual/index.html)，介绍如[编辑器使用](http://docs.qiciengine.com/manual/Interface/index.html)、[界面组件使用](http://docs.zuoyouxi.com/manual/UI/index.html)、[官方插件使用](http://docs.zuoyouxi.com/manual/Plugin/Official.html)和[扩展编辑器](http://docs.zuoyouxi.com/manual/ExtendEditor/index.html)等内容。
- [API手册](http://docs.zuoyouxi.com/api/index.html)，介绍 QICI Core 的类和函数使用
- 例子手册，介绍如何一步步实现具体的游戏例子：
    - [Hello World](http://engine.zuoyouxi.com/demo/GetStart/HelloWorld/docs/index.html)
    - [入门例子](http://engine.zuoyouxi.com/demo/GetStart/StartUp/index.html)
    - [神奇的六边形](http://engine.zuoyouxi.com/demo/Project/tetris/docs/index.html)
    - 更多期待...

## 例子

青瓷引擎提供了众多[游戏例子](http://engine.zuoyouxi.com/demo/)供学习，可直接下载所有[源代码](http://engine.zuoyouxi.com/demo/QICI_Demos.zip)。   

<a href="http://engine.zuoyouxi.com/demo/Project/dota/index.html" target="_blank"><img width='200' src="images/example1.png"></a> <a href="http://engine.zuoyouxi.com/demo/Project/tower/index.html" target="_blank"><img width='200' src="images/example2.png"></a>
<a href="http://engine.zuoyouxi.com/demo/Project/sources/index.html" target="_blank"><img width='200' src="images/example3.png"></a> <a href="http://engine.zuoyouxi.com/demo/misc/performance/index.html" target="_blank"><img width='200' src="images/example4.png"></a>
<a href="http://engine.zuoyouxi.com/demo/misc/widgets/index.html" target="_blank"><img width='200' src="images/example5.png"></a> <a href="http://engine.zuoyouxi.com/demo/Layout/slime/index.html" target="_blank"><img width='200' src="images/example6.png"></a>
<a href="http://engine.zuoyouxi.com/demo/Layout/tablelayout/index.html" target="_blank"><img width='200' src="images/example7.png"></a> <a href="http://engine.zuoyouxi.com/demo/Tilemap/tilemap_Mario/index.html" target="_blank"><img width='200' src="images/example8.png"></a>
<a href="http://engine.zuoyouxi.com/demo/Layout/qq/index.html" target="_blank"><img width='200' src="images/example9.png"></a> <a href="http://engine.zuoyouxi.com/demo/Layout/anchors/index.html" target="_blank"><img width='200' src="images/example10.png"></a>
<a href="http://engine.zuoyouxi.com/demo/ProgressBar/progressBar_mixed/index.html" target="_blank"><img width='200' src="images/example11.png"></a> <a href="http://engine.zuoyouxi.com/demo/UIText/text/index.html" target="_blank"><img width='200' src="images/example12.png"></a>

## 参与

- 青瓷引擎核心: [https://github.com/qiciengine/qiciengine-core](https://github.com/qiciengine/qiciengine-core)
- 青瓷引擎文档: [https://github.com/qiciengine/qiciengine-documentation](https://github.com/qiciengine/qiciengine-documentation)
- 青瓷引擎例子: [https://github.com/qiciengine/qiciengine-examples](https://github.com/qiciengine/qiciengine-examples)
- 青瓷引擎书籍: [https://github.com/qiciengine/qiciengine-cookbook](https://github.com/qiciengine/qiciengine-cookbook)
- 轻量游戏服务器: [https://github.com/qiciengine/qiciengine-server](https://github.com/qiciengine/qiciengine-server)

以上仓库欢迎大家参与提交问题、建议、修正和完善！

目前青瓷引擎的的源代码在发布包的 /lib/qc-core-debug.js 路径，青瓷引擎工程还在内部重构中，我们会尽快发布到 Github 仓库，到时欢迎大家一起参与完善。

## 变更记录

青瓷引擎的所有版本发布历史及变更记录都在论坛的[此贴](http://bbs.zuoyouxi.com/forum.php?mod=viewthread&tid=86&page=1&extra=#pid103)中持续更新。

## 联系我们

- QQ群：214396286
- 问答：[http://wenda.zuoyouxi.com/](http://wenda.zuoyouxi.com)
- 论坛：[http://bbs.zuoyouxi.com/forum.php](http://bbs.zuoyouxi.com/forum.php)
- 官网：[http://www.zuoyouxi.com](http://www.zuoyouxi.com)

## 授权协议

青瓷引擎以 [MIT]((http://opensource.org/licenses/MIT)) 许可授权协议发布。
