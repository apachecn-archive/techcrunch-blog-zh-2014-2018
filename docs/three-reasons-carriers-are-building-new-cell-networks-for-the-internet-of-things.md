# 运营商为物联网构建新蜂窝网络的三个原因 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/10/28/three-reasons-carriers-are-building-new-cell-networks-for-the-internet-of-things/>

丹尼尔·康拉德撰稿人

丹尼尔是

[Beep Networks](https://web.archive.org/web/20230205222955/http://www.beepnetworks.com/)

，是谷歌 Android 和 Access 团队的早期产品经理。

More posts by this contributor

在世界各地，无线运营商正在为物联网构建全新的蜂窝网络。这些新网络无法与手机兼容——它们是为尚不存在的物联网设备设计的。这些也不是小玩家。[康卡斯特](https://web.archive.org/web/20230205222955/https://medium.com/@dconrad/comcast-is-building-an-iot-network-7c4e63e4cafd#.2qe3zrcso)，[软银](https://web.archive.org/web/20230205222955/http://www.softbank.jp/en/corp/group/sbm/news/press/2016/20160912_01/)，[桔子](https://web.archive.org/web/20230205222955/http://www.telecomlead.com/telecom-services/orange-deploys-lora-network-for-iot-in-1300-towns-71246)， [SKT](https://web.archive.org/web/20230205222955/http://www.mobileworldlive.com/asia/asia-news/skt-unveils-pricing-for-lora-based-iot-services/) ， [KPN](https://web.archive.org/web/20230205222955/http://corporate.kpn.com/press/press-releases/the-netherlands-has-first-nationwide-lora-network-for-internet-of-things-.htm) ，[瑞士电信](https://web.archive.org/web/20230205222955/http://www.fiercewireless.com/node/21536)等许多公司正在建设全新的全国性物联网网络。[威瑞森](https://web.archive.org/web/20230205222955/http://www.verizon.com/about/news/verizon-lte-network-technology-iot)和[沃达丰](https://web.archive.org/web/20230205222955/http://www.vodafone.com/content/index/what/technology-blog/enabling-iot.html)正在升级他们的网络，专门为物联网留出频谱。思科、[三星](https://web.archive.org/web/20230205222955/http://news.samsung.com/global/samsung-electronics-to-jointly-build-sk-telecoms-world-first-nationwide-lorawan-network-dedicated-to-internet-of-things)、诺基亚和爱立信正在出售设备使其运转。

新网络是必要的，因为手机网络在三个方面达不到物联网的要求:电池寿命、成本和无线覆盖。

解决其中一个因素就足以证明新网络的合理性。解决所有这三个问题将改变物联网的游戏规则，这也是这些新网络计划要做的。

让我们依次考虑这三个原因。

## 电池寿命:我们需要几年，而不是几天

手机网络并不节能。他们永远也不会。

移动电话网络最初是为汽车电话设计的。协调以 65 英里/小时的速度从一个信号塔“切换”到另一个信号塔——完全不中断电话通话——是使蜂窝网络成为可能的技术突破。这些切换需要复杂的算法以及电话和网络之间的持续通信。

由于这一传统，手机网络上的设备必须每秒钟与信号塔进行多次通信。这对电池寿命来说是非常昂贵的。

为了获得*年*的电池寿命，物联网设备需要大部分时间处于“睡眠”模式，*而不是*使用无线电。手机网络不允许这样。虽然你可能认为你可以关闭设备，然后再打开，但重新连接到手机网络可能会耗费几分钟的电池电量。如果你已经不耐烦地等待你的手机在飞行后重新连接，你知道我在说什么。

物联网的新蜂窝网络采用了不同的方法。

首先，他们使用低功率无线电芯片，优化以最小化数据传输和接收的功率成本。这些系统的功耗通常比蜂窝无线电低一个数量级。

> 超长电池寿命、低成本和无处不在的覆盖范围—所有这些都在一个封装中。

其次，它们允许设备在不接触网络的情况下休眠数分钟或数小时。设备 99.9%的时间处于低功耗模式，唤醒时间仅为数毫秒，以发送或接收数据、读取传感器或激活控制。

这将电池寿命提高了几个数量级。

实现数年的电池寿命对物联网来说是一件大事，因为它有效地消除了安装成本-无需布线，无需充电。物联网可以成为真正的一劳永逸，当您放置数千或数百万设备时，这一点非常重要。

这是一件大事，也是建立新网络的足够理由。

但是还有更多。

## 成本:我们需要便宜的价格

将物联网设备放在手机网络上非常昂贵。

首先，支持物联网设备对蜂窝运营商来说成本高昂。无线频谱耗费数十亿美元，而运营商永远都不够用。每月支付不到一美元的物联网设备将永远不会比拥有 100 美元语音和数据计划的手机获得网络访问优先权。支持物联网设备的机会成本太高。

为了解决这个问题，新的物联网网络要么建立在未经许可的频段上，要么建立在许可蜂窝频谱通道之间相对未使用的“保护频段”上。不管怎样，频谱实际上是免费的。

但是使用手机网络对设备开发者来说也很昂贵。LTE 无线电很复杂，需要多根天线，并且需要昂贵的 IP 许可证。它们价值几十美元。新型物联网网络的芯片组在规模上只需一两美元。

最后，网络认证费用昂贵。例如，在威瑞森的网络上认证一个设备需要花费 5 万到 10 万美元，而这个过程需要几个月。认证是必要的，因为有缺陷的设备可能会干扰威瑞森网络上的手机。他们小心谨慎是有道理的。

新的物联网网络被设计为对干扰具有鲁棒性，因为它们被设计为在干扰是常态的共享频带中运行。在许多情况下，最终用户可以免费设置自己的网关，就像 Wi-Fi 接入点一样。

这就引出了下一点。

## 覆盖范围:我们到处都需要它

事实是，LTE 并非无处不在。物联网设备有一个令人讨厌的趋势，那就是被部署在当今手机网络覆盖不到的地方:比如地下室的洪水探测器、地下停车场的停车传感器和农村玉米田的土壤传感器。

新的物联网网络以两种不同的方式处理覆盖问题。

首先，网络被优化以最大化室内深度渗透，而不是带宽。射频调制的一个基本规则是，你可以通过传输许多比特来表示一个比特，从而用范围换取带宽。虽然 LTE 针对数据饥渴的智能手机进行了优化，但新的物联网网络针对短消息进行了优化——比如，传感器读数或设置恒温器的命令。在相同的功率水平下，它们将获得更大的覆盖范围，尽管比特率通常低于 1 Kbps。

其次，在某些情况下，网关可以自我部署，就像 Wi-Fi 路由器一样。因此，如果你的本地运营商不能到达你的地下室，你可以在附近放下你自己的网关，让它上线。自部署网络对于这些技术的推广至关重要，尤其是在运营商运营网络仍在推广的早期。

这就是 IoT 实际上是如何发生的。长电池寿命、低成本和无处不在的覆盖范围—所有这些都在一个封装中。

我花了数年时间研究联网设备，对我来说，这听起来像是圣杯。它意味着一劳永逸的设备，在任何地方都可以工作。

我等不及了。