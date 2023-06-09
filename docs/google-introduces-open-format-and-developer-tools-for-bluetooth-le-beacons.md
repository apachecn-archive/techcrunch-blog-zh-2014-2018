# 谷歌推出新的开放格式和开发工具，用于与 BLE Beacons TechCrunch 合作

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/07/14/google-introduces-open-format-and-developer-tools-for-bluetooth-le-beacons/>

谷歌今天[推出了](https://web.archive.org/web/20221007102112/http://googledevelopers.blogspot.com/2015/07/lighting-way-with-ble-beacons.html)一系列围绕蓝牙低能耗(BLE)信标的新产品，试图挑战苹果的 [iBeacon](https://web.archive.org/web/20221007102112/https://developer.apple.com/ibeacon/) 生态系统。

这些新产品包括新的开放 beacon 格式、用于在 beacon 上构建应用和服务的工具和 API，以及用于管理和监控大型 beacon 部署的新的以开发人员为中心的服务。

众所周知，谷歌对蓝牙信标很感兴趣。大约一年前，我们[第一次听说了](https://web.archive.org/web/20221007102112/http://www.infoworld.com/article/2608498/mobile-apps/what-you-need-to-know-about-using-bluetooth-beacons.html)谷歌的附近项目，例如，它今天也作为 API 发布。而 Nearby 也使用其他信号(WiFi、音频等。)，BLE 信标显然是谷歌努力的中心。

谷歌的第一个新 beacon 产品——也是其其他计划的基石——是 Eddystone 格式(如果你想知道的话，以一个英国灯塔命名[。正如谷歌产品经理马修·库里克(Matthew Kulick)本周早些时候告诉我的那样，这种新格式是该公司今天在 Github 上发布的 Apache 2.0 开源许可证，旨在为开发人员提供一种更强大、更可扩展的信标工作方式。](https://web.archive.org/web/20221007102112/https://en.wikipedia.org/wiki/Eddystone_Lighthouse)

谷歌已经与信标硬件供应商合作，如 [Bluvision](https://web.archive.org/web/20221007102112/http://bluvision.com/beeks-beacons/) 、 [Estimote](https://web.archive.org/web/20221007102112/http://estimote.com/) 、 [Kontakt.io](https://web.archive.org/web/20221007102112/http://kontakt.io/) 、 [Radius Networks](https://web.archive.org/web/20221007102112/http://www.radiusnetworks.com/) 和 [Signal360](https://web.archive.org/web/20221007102112/http://www.signal360.com/) 将 Eddystone 格式内置到他们的设备中。新格式是完全平台无关的(只要设备支持 BLE，它就支持 Eddystone ),任何现有的信标都可以通过固件更新与 Eddystone 兼容。

在 API 方面，谷歌今天为希望在应用中使用信标的开发者发布了两个新的 API。Android 和 iOS 的附近 API 现在使应用程序更容易找到附近的设备和信标并与之通信。这可能是一个艺术展览或一个公共汽车站(谷歌已经[与波特兰的交通部门](https://web.archive.org/web/20221007102112/http://www.oregonlive.com/commuting/index.ssf/2015/03/trimet_google_activate_wireles.html)合作，或实现这一点)。

邻近信标 API 则更进一步，帮助开发人员将位置和相关数据与信标相关联。这些数据储存在谷歌的服务器上。

谷歌用于灯塔车队管理的新工具也是新的。“我们希望让你的信标辅助应用从试点转向规模化变得更容易，”Kulick 说。例如，当你在一个体育场使用大量的信标时，事情很快就变得具有挑战性。Kulick 指出，仅仅获得每个信标的状态就可能很难。这项新服务位于谷歌的 Eddystone 遥测框架之上，开发人员可以利用这些数据，在从中获得的数据基础上构建自己的服务和仪表板。不过，就目前而言，谷歌不会提供自己的仪表盘。该公司告诉我，它没有计划对这项服务收费。

当然，谷歌自己的产品也会利用这项新技术。波特兰的谷歌地图用户从今年早些时候开始能够获得基于信标的交通通知，很快，Google Now 也将能够使用这项服务来提供上下文信息，例如，当你在餐馆时，你将能够在 Google Now 中看到菜单(尽管当你在餐馆时，你真的真的应该[放下手机](https://web.archive.org/web/20221007102112/http://www.bbc.com/news/blogs-echochambers-28272380)……)。