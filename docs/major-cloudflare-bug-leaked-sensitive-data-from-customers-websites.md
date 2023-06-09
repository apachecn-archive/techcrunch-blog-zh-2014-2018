# 重大 Cloudflare bug 从客户网站泄露敏感数据

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/23/major-cloudflare-bug-leaked-sensitive-data-from-customers-websites/>

Cloudflare 今天披露了其软件中的一个严重错误，该错误导致密码、cookies、身份验证令牌等敏感数据以明文形式从其客户的网站上泄漏。[公告](https://web.archive.org/web/20230315223416/https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/)是对内容交付网络的一个重大打击，该网络为超过 500 万个网站提供增强的安全性和性能。

这可能允许任何注意到错误的人收集各种非常私人的信息，这些信息通常是加密的或模糊的。

补救措施因另一个问题而变得复杂。其中一些数据是由搜索引擎自动缓存的，这使得清理善后工作变得尤为困难，因为 Cloudflare 不得不联系谷歌、必应、雅虎和其他搜索引擎，要求他们手动清除数据。

该漏洞可能早在 2016 年 9 月 22 日就已经活跃，比谷歌 Project Zero 的一名安全研究员发现它并向 Cloudflare 报告的时间早了近五个月。

然而，最严重的泄漏发生在 2 月 13 日和 2 月 18 日之间，当时大约每 3，300，000 个对 Cloudflare 站点的 HTTP 请求中就有 1 个会导致数据泄露。攻击者可以实时访问数据，或者稍后通过搜索引擎缓存访问数据。

Cloudflare 在其发布的问题公告中指出，即使在高峰期，数据也只在大约 0.00003%的请求中泄露。这听起来没什么，但 Cloudflare 的大规模客户群包括像约会网站和密码管理器这样的类别，这些网站托管着特别敏感的数据。

Cloudflare 首席技术官 John Graham-Cumming 告诉 TechCrunch 说:“在高峰时期，我们每天会因为一个请求而泄露 12 万条信息。他强调说，并非所有泄露的信息都包含秘密信息。“里面的东西是随机的，因为它是随机存储器，”他说。

该错误发生在一个 HTML 解析器中，Cloudflare 使用该解析器来提高网站性能——它准备在谷歌的发布平台 AMP 中分发网站，并将 HTTP 链接升级到 HTTPS。Cloudflare 的三个功能([电子邮件混淆](https://web.archive.org/web/20230315223416/https://support.cloudflare.com/hc/en-us/articles/200170016-What-is-Email-Address-Obfuscation-)、[服务器端排除](https://web.archive.org/web/20230315223416/https://support.cloudflare.com/hc/en-us/articles/200170036-What-does-Server-Side-Excludes-SSE-do-)和[自动 HTTPS 重写](https://web.archive.org/web/20230315223416/https://support.cloudflare.com/hc/en-us/articles/227227647-How-do-I-use-Automatic-HTTPS-Rewrites-))没有通过解析器正确实现，导致随机数据块暴露。

最终，甚至 Cloudflare 本身也受到了这个 bug 的影响。Graham-Cumming 在 Cloudflare 的公告中写道:“一个明显的信息泄露是用于保护 Cloudflare 机器之间连接的私钥。”。加密密钥允许该公司自己的机器安全地相互通信，并于 2013 年实施，以回应对政府监控的担忧。

Graham-Cumming 强调，Cloudflare 没有发现黑客发现或利用该漏洞的证据，并指出，如果攻击者试图访问特定网站的数据，Cloudflare 会发现他们网络上的异常活动。

“这是理解 HTML 的一个错误，”格雷厄姆-卡明解释说。“我们理解对网页的即时修改，它们会通过我们。为了做到这一点，我们在计算机内存中有网页。你可能会越过网页的末尾，进入你不应该看到的内存。”

Cloudflare 在旧金山和伦敦的团队相互交接工作，一旦发现漏洞，就昼夜不停地修复。他们在七个小时内阻止了最严重的问题。该公司花了六天时间完全修复了这个漏洞，并与搜索引擎合作清除数据。

谷歌工程师塔维斯·奥曼迪首先注意到了这个漏洞，他开玩笑地称之为“云出血”,指的是心脏出血漏洞。他在[的一篇博客文章](https://web.archive.org/web/20230315223416/https://bugs.chromium.org/p/project-zero/issues/detail?id=1139)中说，他在一个项目中遇到了意想不到的数据，起初他怀疑自己的代码中是否有 bug。经过进一步测试，他意识到泄漏来自 Cloudflare。

“我们提取了一些实时样本，我们观察到了加密密钥、cookies、密码、大量帖子数据，甚至其他用户对其他主要 Cloudflare 托管网站的 HTTPS 请求，”奥曼迪写道。“这种情况是不寻常的，[个人身份信息]在正常使用期间被爬虫和用户主动下载，他们只是不明白他们看到了什么。”奥曼迪补充说，他后来销毁了这些样本，因为它们包含敏感信息，但他贴出了从优步、Fitbit 和 OkCupid 泄露的一些信息的编辑截图。

除了奥曼迪收集的样本，还不清楚可能泄露了什么其他信息。“这很难说，因为这种信息是短暂的，”格雷厄姆-卡明说。但是奥曼迪说他的样本揭示了高度敏感的数据。

“我们不断发现更多需要清理的敏感数据。直到这次事件，我才意识到 Cloudflare CDN 背后有多少互联网，”奥曼迪写道。“我发现了来自主要交友网站的私人信息、来自一家知名聊天服务的完整信息、在线密码管理器数据、来自成人视频网站的帧、酒店预订。我们谈论的是完整的 HTTPS 请求、客户端 IP 地址、完整的响应、cookies、密码、密钥、数据，一切。”

尽管 Cloudflare 与奥曼迪合作解决这个问题，但他认为该公司关于此事的最终博客帖子“严重低估了客户的风险”奥曼迪还对 Cloudflare 未能在补救过程中加快步伐表示失望。

但是 Graham-Cumming 说，Cloudflare 不可能比现在运行得更快。Graham-Cumming 还表示，奥曼迪在审阅一份拷贝时，称 Cloudflare 的披露“完全可以接受”。

“这要经过 90 天的披露。格雷厄姆-卡明说:“我们在六天后才披露。”。“他说他很沮丧，但我有点困惑，为什么他对 6 天而不是 90 天感到沮丧。我们本应该更早披露，但是因为一些信息已经被缓存，我们认为我们有责任在公开之前清理这些信息。信息会在谷歌这样的搜索引擎中持续存在，这是一种危险。”

Graham-Cumming 说，像优步和 OkCupid 这样的 Cloudflare 客户没有直接得到数据泄露的通知，因为这种情况涉及到安全风险。“Cloudflare 之外没有后门通信——只有与谷歌和其他搜索引擎的通信，”他说。