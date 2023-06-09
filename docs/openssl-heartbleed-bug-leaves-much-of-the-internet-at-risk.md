# OpenSSL Heartbleed Bug 使大部分互联网处于危险之中 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/04/08/openssl-heartbleed-bug-leaves-much-of-the-internet-at-risk/>

互联网的一大块正在[崩溃](https://web.archive.org/web/20221006233926/https://beta.techcrunch.com/2014/04/07/massive-security-bug-in-openssl-could-effect-a-huge-chunk-of-the-internet/)。OpenSSL 被许多公司和服务用来加密他们的数据，它包含一个长达两年的缺陷，如果被利用，它允许外部各方从服务器的工作内存中提取 64 千字节的数据。

这并不多，但这是一个非常可重复的利用，这意味着邪恶的各方可以一次又一次地点击 64 千字节的按钮。最终，据推测，您将得到金奖券:私有加密密钥。有了它，你就可以解密敏感的、受保护的数据，没有人会知道。

这就是为什么情况比您最初想象的还要糟糕:即使您修补了 OpenSSL，您也不知道您的服务器之前是否受到了威胁。你可以扔掉旧的密钥，生成新的密钥，但这只能保护你继续前进。

安全研究员，【Nicholas Weaver 说了下面的:“我打赌一年后会有很多易受攻击的服务器。这不会得到解决。”事情很少像人们说的那样糟糕。这是其中的一次。

另一个警告:如果你存储了加密流量池，然后设法通过 Heartbleed bug 提取数据的密钥，所有过去的流量都将变得可利用。引用马蒂亚斯·拜恩斯的话，另一种安全类型:“ಠ_ಠ.”拜恩斯还指出，使用完全前向保密加密的数据不会有风险，这对一些人来说是一种安慰。

谁有能力收集和存储这些信息？比如国家安全局。该组织因窃听互联网的核心电缆，甚至监视数据中心内的企业流量而臭名昭著。包括，你会记得，雅虎在欧洲的数据中心。雅虎是受到攻击威胁的一方。你算算。雅虎最近宣布，它已经加强了数据中心内部和数据中心之间的加密。

在一份电子邮件声明中，雅虎告诉 TechCrunch 以下内容:

> 一个名为 Heartbleed 的漏洞最近被发现影响了许多使用 OpenSSL 的平台，包括我们的平台。我们一意识到这个问题，就开始着手解决它。我们的团队已经成功地
> 对主要的雅虎网站(雅虎
> 主页、雅虎搜索、雅虎邮件、雅虎财经、雅虎体育、雅虎
> 食品、雅虎科技、Flickr 和 Tumblr)进行了适当的修正，我们现在正在努力对其余网站实施
> 修正。我们致力于为全球用户提供最安全的体验，并持续努力保护用户数据。

这不是最近唯一的加密灾难。NSA [花了一大笔钱](https://web.archive.org/web/20221006233926/https://beta.techcrunch.com/2013/12/20/nsa-reportedly-paid-a-security-firm-millions-to-ship-deliberately-flawed-encryption-technology/)让 RSA 采用一个可被利用的随机数生成器。这件事很严重。如果美国国家安全局不停止大规模收集数据，以及其他国家的类似机构，加密工作就很重要。

如果没有，没有人有隐私。

***更新:**微软向 TechCrunch 提供了以下声明:“我们正在关注 OpenSSL 库问题的报告。如果我们确定我们的设备和服务受到影响，我们将采取必要措施保护我们的客户。”*

图片由 FLICKR 用户 Jon Robson 在 [CC BY 2.0](https://web.archive.org/web/20221006233926/http://creativecommons.org/licenses/by/2.0/) 许可下(图片已被裁剪)