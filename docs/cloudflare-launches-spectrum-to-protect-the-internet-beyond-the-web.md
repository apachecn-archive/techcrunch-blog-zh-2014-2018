# Cloudflare 推出 Spectrum 保护网络之外的互联网

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/04/12/cloudflare-launches-spectrum-to-protect-the-internet-beyond-the-web/>

当它在 2010 年推出时， [Cloudflare](https://web.archive.org/web/20230225041631/http://www.cloudflare.com/) 的宗旨就是提高网站速度，保护网站免受黑客攻击。今天，随着[推出](https://web.archive.org/web/20230225041631/http://blog.cloudflare.com/spectrum/)[频谱](https://web.archive.org/web/20230225041631/https://www.cloudflare.com/products/cloudflare-spectrum/)的，它迈出了一大步，超越了网络，进入保护——并可能加速——互联网的其他部分。

虽然 Cloudflare 的常规服务适用于应用程序、API 和网站，所有这些都倾向于使用常规的 web 协议，但 Spectrum 是关于所有其他在互联网上移动的流量。或者如该公司所说:Spectrum 将 Cloudflare 扩展到 65，533 个端口。

需要明确的是，这并不是像 Cloudflare 的大多数现有服务那样的自助式产品。它也主要是关于安全性，而不是性能(虽然有点偶然，它也经常加快连接)。这在很大程度上是一款面向大型企业的产品，这些企业希望确保其各种服务处于安全连接的背后。

正如 Cloudflare 联合创始人兼首席执行官马修·普林斯(Matthew Prince)告诉我的那样，该公司从保护网站开始，部分原因是它在成立初期一直在追逐小客户。而那些客户当时大多在建网站。随着公司客户群的增长，这些客户从小型网站转向了更高级的网络应用和移动应用。Cloudflare 正在与最大的金融机构和其他主要企业客户进行沟通，他们开始要求不仅仅是保护其网站的服务。

普林斯指出:“对于生于网络的公司来说，我们做得很好，但如果你是一家大型金融机构，你利用网络做的很多事情并不在网络上。”

借助 Spectrum，这些公司现在可以将其内部电子邮件服务器、预订引擎、物联网设备甚至游戏服务器置于 Cloudflare 的网络之后，以保护他们免受 DDoS 攻击和其他安全风险。事实上，普林斯指出，他认为游戏公司将是这项服务的早期采用者之一，因为他们往往不得不应对常规的 DDoS 攻击。

“Hypixel 是 Mirai 未来组合僵尸网络 DDoS 攻击的第一批目标之一，经常受到大规模攻击，”《我的世界》服务器专家 Hypixel 的首席技术官 Bruce Blair 说。“在使用 Spectrum 之前，我们不得不依赖不稳定的服务和技术，这增加了延迟，恶化了用户体验。现在，我们能够在不增加延迟的情况下持续受到保护，这使它成为任何延迟和正常运行时间敏感型服务(如在线游戏)的最佳选择。”

Prince 还指出，这些用户还可以选择加密他们的流量——这是许多传统协议不支持的。

由于流量随后通过 Cloudflare 的网络进行路由，这些连接通常也比以前更快。虽然情况并不总是如此，但 Prince 强调也不需要支付性能损失。由于这种将在频谱中移动的流量，Cloudflare 无法通过在边缘缓存内容来提高网站速度，但话说回来，这里的卖点是安全性，而不是速度。

想要注册这项服务的企业现在可以使用 Spectrum。Cloudflare 没有公布任何定价计划，但普林斯告诉我，该公司将根据公司通过该服务发送的流量收取费用。