# 2016 年和未来一年

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/12/29/2016-and-the-year-ahead/>

约翰-卡明撰稿人

约翰·格雷厄姆·卡明是

[Cloudflare](https://web.archive.org/web/20230225042442/https://www.cloudflare.com/)

.

过去的一年是互联网攻击、加密、停电、速度和物联网的重要一年，2017 年将为这些问题带来更多头条新闻。随着 Cloudflare 为来年做准备，我们对互联网的未来做了一些预测。

但首先，让我们回顾一下 2016 年互联网广泛使用和滥用的结果。

在加蓬和冈比亚，互联网连接在选举期间中断。冈比亚[有争议的选举始于持续了很短时间的网络中断。在加蓬，互联网关闭持续了几天。就在我们写这篇文章的时候，像刚果民主共和国这样的国家正在讨论封锁特定的互联网服务，显然忘记了在这些其他国家吸取的教训。](https://web.archive.org/web/20230225042442/https://www.amnesty.org/en/latest/news/2016/12/gambia-communication-blackout-shatters-illusion-of-freedom-during-the-election/)

DDoS 攻击全年持续不断，攻击大大小小的网站。在 3 月份，我们看到周末的 DDoS 攻击达到了 400 Gbps 的峰值，而在 12 月份，我们看到了一种新的攻击者模式，他们将攻击视为朝九晚五的常规工作。

除了真正的 DDoS，还有来自一个自称为 [Armada Collective](https://web.archive.org/web/20230225042442/http://www.theverge.com/2016/4/26/11512032/ddos-ransom-armada-collective-denial-of-service-threat) 的组织的空洞威胁，要求网站和 API 使用比特币来保持在线。另一组突然冒出来[跟风](https://web.archive.org/web/20230225042442/https://security.radware.com/ddos-threats-attacks/threat-advisories-attack-reports/ransom-attacks/)同样的作案手法。

物联网变成了许多人曾经警告过的东西:用于攻击的设备大军。一个由物联网摄像头组成的僵尸网络大军和一次重大攻击干掉了 DNS 服务提供商 [Dyn](https://web.archive.org/web/20230225042442/https://en.wikipedia.org/wiki/2016_Dyn_cyberattack) 。

非 DDoS 攻击继续快速发展，需要 WAF 保护的黑客如 httpoxy 和 ImageTragick 对未受保护的站点造成破坏。TLS 经历了又一次被称为[淹没](https://web.archive.org/web/20230225042442/https://en.wikipedia.org/wiki/DROWN_attack)的攻击。

> 随着 web 变得更加加密，同时优化 TLS 和 TCP 的需求变得更加重要。

但这并不完全是悲观的。IPv6 见证了巨大的移动流量，突然感觉绝对真实。苹果宣布 iOS 应用程序必须支持纯 IPv6 网络，主要的互联网服务提供商开始优先考虑 IPv6 流量。TLS 1.3 的上线极大地简化和提高了互联网的安全性。

随着对 HTTP/2 的广泛支持，包括服务器推送和 WebP 转换，互联网变得更快了。随着 web 变得越来越加密，同时优化 TLS 和 TCP 的需求变得越来越重要，Cloudflare 通过 Origin CA、无处不在的 HTTPS 以及为每个人提供受保护的 WebSockets 帮助提高了安全性。

## 未来一年

我们的团队由工程师、程序员、密码学家和黑客组成，他们看了看虚拟水晶球，得出了我们对 2017 年的预测。以下是我们认为未来一年必须提供的内容。

**1Tbps DDoS 攻击将成为“大规模攻击”的基准**

四年前，我们在一篇关于 65Gbps DDoS 的博客文章中用 band Massive Attack 的图片进行了说明。第二年，[大规模攻击](https://web.archive.org/web/20230225042442/https://en.wikipedia.org/wiki/Massive_Attack)卷土重来，引发 300Gbps 攻击；随着全球网速的提高，DDoS 的规模也在扩大。2016 年，我们已经零星地看到来自各种服务提供商的 1Tbps DDoS 攻击报告。我们认为，2017 年，massive attack 的基线将是 1Tbps(我们希望 Massive Attack 2016 年的歌曲发行预示着 2017 年的专辑)。

**随着像 QUIC 这样的协议越来越流行，互联网将再次变得更快**

尽管 HTTP/2 对 web 性能有很大的影响，但它也依赖 TCP 协议进行连接，这可能会在有损耗的网络上导致性能问题。谷歌一直在试验一种叫做 [QUIC](https://web.archive.org/web/20230225042442/https://en.wikipedia.org/wiki/QUIC) 的协议，它使用 UDP 而不是 TCP。我们希望这种基于 UDP 的 web 协议实验能够继续下去，并成为主流。

**IPv6 将成为移动网络的事实，只有 IPv4 的固定网络将被视为过时**

我们的数据显示 IPv6 快了 27%，脸书说快了 10%到 15%，LinkedIn 说移动设备快了 10%到 40%。不管你相信哪个数字，很明显 IPv6 提供了速度优势。与此同时，ISP 和移动网络正在推动 IPv6 的更大部署，我们预计 IPv6 将在 2017 年成为所有网络的规范。特别是对于移动网络，我们认为 IPv4 将被弃用。

该图表显示了 25，000 个通过 IPv6 访问的网站(根据 Alexa)的百分比:

**阿沙一号将宣布碰撞**

早在 1996 年，MD5 中的潜在冲突就被发现了，但直到 2005 年才出现真正的冲突。当时，MD5 和 SHA-1 的死亡都被预测到了。MD5 现在被认为在密码学上毫无用处，甚至被恶意软件用来伪造证书。

自 2005 年以来，关于 SHA-1 的碰撞阻力的坏消息一直在收集，我们预测实际的碰撞将在 2017 年计算出来。

**第 7 层攻击将会上升，但第 6 层也不会太远**

当人们想到 DDoS 攻击时，他们通常会想到针对第 3 层和第 4 层的容量攻击(如 SYN floods)。我们认为，第 7 层攻击(特别是针对 HTTP 和 DNS 协议的攻击)将在 2017 年继续上升，因为攻击者正在寻找超越简单体积攻击的智能方法来使 web 应用程序离线。

同时，针对 TLS 协议的第 6 层攻击将会出现。我们在过去已经看到过这种攻击(通过要求缓慢或复杂的加密操作来消耗服务器 CPU 的攻击)，聪明的攻击者将继续搜索 web 应用程序或协议实现中的任何弱点。

**到今年年底，移动流量将占全部互联网流量的 60%**

早在 2014 年，移动互联网用户的数量就超过了固定互联网用户，如今超过 80%的互联网用户拥有智能手机，而他们 89%的移动时间都花在了使用应用上。

这意味着加速和保护 API(应用程序用于互联网连接)至关重要，趋势表明今年移动流量将占所有互联网流量的 60%。这种向移动的转变比以前更加强调优化的网络体验和健壮的 API。

**域名系统的安全性将受到重视**

对 Dyn DNS 服务的攻击表明，互联网中一个经常被忽视的部分——域名系统——对其运行至关重要。在 Dyn 攻击之前，许多关于 DDoS 攻击的新闻都集中在网站和网络攻击上。随着对 DNS 至关重要性的认识，其安全性将在 2017 年受到重视，保护 DNS 基础设施和服务器将成为一项业务需求。

同时，DNS 的开放性将成为焦点，DNSSEC 将在保护 DNS 免受攻击方面发挥更大的作用。