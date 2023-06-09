# 中国程序员在 iPhone 6 Plus 上安装 Windows 95 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2014/11/10/chinese-programmer-sticks-windows-95-on-an-iphone-6-plus/>

# 中国程序员将 Windows 95 安装在 iPhone 6 Plus 上

今天在“把东西放到不属于它们的东西上”中，我们呈现一个用户， [xyq058775](https://web.archive.org/web/20230129063911/http://bbs.feng.com/read-htm-tid-8563343.html) ，以及他令人兴奋的承认他在一部全新的 iPhone 上安装了 Windows 95。他使用了一个叫做 [iDos](https://web.archive.org/web/20230129063911/https://itunes.apple.com/cg/app/idos/id377135644?mt=8) 的工具，一个开源的类似 DOSBox 的应用程序来安装操作系统。他发现大部分功能都运行良好，但他无法升级到 Windows XP。我们可以假设他也能玩[末日](https://web.archive.org/web/20230129063911/http://doom.wikia.com/wiki/Doom95)。

这整个过程没有什么新意——从最初的 VAX 机器开始，人们就已经在事物上放置了模拟器——但是看到复活的软件在新硬件上如此容易地运行，这很酷。虽然我无法想象这方面的真实用例(也许您真的需要运行 Mavis Beacon 的副本？)这是一个很好的理论练习。谁知道呢，说不定下一个就有人能跑 [POSDT 了。](https://web.archive.org/web/20230129063911/https://techcrunch.com/2008/03/15/juvenalia-posdt-and-bigwidelogic/)

以下是翻译得不好的常见问题:

￼1.问:我可以安装 WINDOWS XP 吗？答案是肯定的，你可以，但肯定不能

[idos](https://web.archive.org/web/20230129063911/http://toucharcade.com/2010/10/26/idos/)

因为 idos 只是简单的模拟 dos 环境，并不是真正意义上的虚拟机，所以系统运行起来比较困难，DOS 和 idos 模拟环境又不具备运行 XP 的基本环境需求，所以以后如果移植 XP 系统，那么我会利用闲暇时间跟朋友们一起在 ios 平台上写一个运行 XP 虚拟机系统的插件。

2.问:你为什么要这样做？为什么不用远程桌面。答:首先说明一下，远程桌面这种东西目前在 win98 系统上是不支持的，不要在系统安装期间使用，工具方法都发过来了。

3.问:为什么我安装 explorer 的进程是错误的？答:因为 idos 模拟器只模拟了 16 位的 dos 环境，虽然 win98 是 16/32 混合系统但是 Explorer 和 exe 进程很大一部分需要的是 32 位环境，所以当它们需要 32 位程序调用一些系统环境变量和支持库时会出现错误，LZ 修改一些资源的目的是让他在 idos 环境中运行良好，但是，这种修改会改变部分机器，从而导致一些设备在使用 LZ 修改良好的映像时出现错误。以后 LZ 会根据大家的反馈慢慢完善！

如果你能看懂中文的话，他的帖子上有完整的说明。如果没有，我把安装留给读者作为练习。

![0238ef6bbd9be53a](img/4a395f3ab92c4107ff1750ae4c959c30.png)

![183048vvy0yrafqdvbvupf](img/515659df97391fdc97e54bab71f45562.png)

![155633w2jcu1go2oy1cycq](img/05fad171b140210abd41232d42129273.png)