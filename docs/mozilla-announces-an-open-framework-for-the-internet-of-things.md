# Mozilla 宣布开放物联网网关 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/06/mozilla-announces-an-open-framework-for-the-internet-of-things/>

苹果、谷歌、亚马逊和三星都在努力创建自己的标准来控制你家中所有的联网设备。Mozilla [刚刚宣布](https://web.archive.org/web/20230220110828/https://blog.mozilla.org/blog/2018/02/06/announcing-project-things-open-framework-connecting-devices-web/)任何人现在都可以创建一个开放的网关来控制物联网。该组织还证实，它仍在制定一套框架和开放标准，以便我们不会最终拥有由大型科技公司控制的物联网。

联网设备很棒，直到你意识到你的联网恒温器只能与亚马逊 Echo 一起工作，你的联网灯泡只能与 Siri 和 Home 应用程序一起工作。

配件制造商也不一定希望少数大型科技公司控制物联网。科技巨头最终可能会收取昂贵的许可费来与他们的生态系统合作。客户最终不得不做出艰难的决定。

Mozilla 是开放网络的大力支持者。因此，这家非营利组织制定联网设备计划似乎是很自然的。[项目事物](https://web.archive.org/web/20230220110828/https://iot.mozilla.org/)包含多个项目，所以让我们看看 Mozilla 的工作。

首先，Mozilla 希望与 W3C 一起围绕[物联网](https://web.archive.org/web/20230220110828/https://iot.mozilla.org/wot/)创建一个开放标准。这个想法是，配件制造商和服务提供商应该使用相同的标准，使设备互相交谈。这些规范依赖于 JSON、REST 和 WebSockets API。这些是网络上的标准数据和 API 模型，它们应该可以很好地适用于联网设备。

第二，Mozilla 正在开发一个物联网网关，这样你就可以用一个开放的设备替换你的亚马逊 Echo、飞利浦 Hue hub、苹果电视和谷歌 Home。你已经可以[使用 Raspberry Pi 3、ZigBee 和 Z-Wave USB 加密狗创建一个网关](https://web.archive.org/web/20230220110828/https://hacks.mozilla.org/2018/02/how-to-build-your-own-private-smart-home-with-a-raspberry-pi-and-mozillas-things-gateway/)。

最终，制造商可以利用这项工作来创建自己的网关。也许 Netgear 可以在他们的下一个路由器中嵌入一个物联网网关——你的路由器连接到互联网，毕竟是全天候运行的。开发者还可以在 HomeKit API 或亚马逊的智能家居技能 API 之间建立桥梁，这样所有设备都可以与你的亚马逊 Echo、谷歌 Home 或 iPhone 一起工作，而无需太多努力。物联网可能成为这些专有 API 之间的通用语言。

最后，Mozilla 正在创建一个界面来控制你的连接设备。你可以将 Mozilla 的 progressive web 应用程序添加到智能手机主屏幕上，并控制你的家。例如，你可以用你的声音来开灯，创建 IFTTT 风格的规则来自动化你的房子，添加平面图来布置你的设备等等。

Mozilla 设计了一个附加系统，这样你就可以通过安装插件来增加对新设备和协议的支持。需要注意的是，所有这些都是在你家里自己的网关上运行的。当你用语音开灯时，谷歌或亚马逊看不到。

最终，我还可以看到应用开发者利用物联网协议创建本地应用来控制你的房子。但很明显，Mozilla 想从各个角度攻击这个问题。开发人员已经可以开始摆弄项目的东西，并为开发做出贡献。