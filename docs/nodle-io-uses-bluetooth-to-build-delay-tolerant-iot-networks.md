# Nodle.io 使用蓝牙构建延迟容忍物联网网络 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/07/12/nodle-io-uses-bluetooth-to-build-delay-tolerant-iot-networks/>

随着物联网(IoT)设备的数量继续呈指数级增长，我们也需要合适的网络来将这些设备相互连接并连接到更广泛的互联网，这一点变得越来越明显。如今的标准程序是使用内置的 3G 或 4G 卡，这使得设备体积庞大，或者像 [LoRa](https://web.archive.org/web/20221025223006/https://www.lora-alliance.org/) 或 [Sigfox](https://web.archive.org/web/20221025223006/https://www.sigfox.com/en) 这样的低功耗广域网。[本周发布的 Nodle.io](https://web.archive.org/web/20221025223006/http://nodle.io/#/landing) 采用了一种不同的方法，使用基于软件的蓝牙网络，该网络使用数十亿现有物联网设备中已有的硬件，结合[智能手机和应用](https://web.archive.org/web/20221025223006/https://play.google.com/store/apps/details?id=io.nodle.noodle&rdid=io.nodle.noodle)来连接设备。

该公司由 Micha Benoliel 创建，他之前与人共同创建了 Open Garden，这是一家初创公司，入围了我们的 Disrupt New York 2012 战地竞赛，专注于在连接很少或没有连接的地区为手机提供网状网络。Benoliel 于 2016 年初卸任 Open Garden 首席执行官，随后于去年年底彻底离开公司。虽然 Open Garden 的重点是手机和在手机上运行的应用程序，但 Nodle.io 完全专注于物联网。Nodle 肯定与 Open Garden 分享了它的一些核心理念——特别是它如何实现众包连接。

Nodle 的承诺是，这种网络将能够提供与 Sigox 和 LoRa 相当的带宽，但物联网设备本身的能源需求明显更低。为了实现这一目标，Nodle 将赌注压在了众包带宽和合作伙伴关系的结合上。

Benoliel 强调，这里的网络原理不同于 Open Garden 所研究的网状网络。这里的转折是，Nodle 将为希望将 Nodle SDK 构建到应用程序中的开发人员(和电信公司)提供一个 SDK。这是因为 Nodle 网络仍然需要一种方法来连接到互联网。使用其 SDK 的开发者可以通过将他们的用户转化为潜在的网络中心，使 Nodle networks 可以用来连接互联网，从而从他们的应用中获利。然后，Nodle 根据这些开发者促成的连接数量与他们分享收入。

![](img/794aeb59506a951be25545036988dd17.png)

因为我们基本上是在谈论使用众包将设备连接到互联网，所以这种网络显然不适合实时访问数据至关重要的应用程序。

这是与网状网络不同的网络原理。贝诺里埃尔说，这被称为“延迟容忍网络(DTL)”通过 Nodle，SDK 直接从周围的设备收集数据，当智能手机通过免费 WiFi 连接到互联网时，数据就会被发送到云端。随着图书馆智能手机密度的增加，网络变得越来越实时。一些电信公司也表示有兴趣租用他们的 3G 和 4G 基础设施。在这种情况下，数据通过他们的网络被发送到云端。"

该团队还推出了一款面向 Android 的智能手机应用程序( [Noodle](https://web.archive.org/web/20221025223006/https://play.google.com/store/apps/details?id=io.nodle.noodle) )，这基本上是一款支持 Nodle 的应用程序，每当用户从 Nodle 物联网设备收到 ping 命令时，就会奖励用户一个“Noodle”。目前这样做没有奖励，但该应用程序有一个排行榜。

Benoliel 说，Nodle SDK 也可以与来自运营商和原始设备制造商的广告 SDK 一起工作。“不过，一个主要的区别是:我们不需要了解用户的任何信息。我们对用户数据不感兴趣，设备 id 也是匿名的，”他说。

尽管该公司本周才在香港的 RISE 大会上正式推出，但该团队已经与 Stilla 和 Trackr 等物联网制造商以及 DevicePilot 等 LifeKit 和物联网平台支持者建立了合作关系。

虽然 Nodle 开始利用智能手机基础设施，但计划将它扩展到家用路由器，甚至汽车等交通工具。

[![](img/63eea429aa686e1b03df7c43f4ded04f.png)](https://web.archive.org/web/20221025223006/https://beta.techcrunch.com/wp-content/uploads/2017/07/dashboard_deviceslocations_b.jpg)