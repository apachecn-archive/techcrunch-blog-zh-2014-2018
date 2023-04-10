# 消息应用 Wire 现在对其 e2e 加密技术进行了外部审计

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/10/messaging-app-wire-now-has-an-external-audit-of-its-e2e-crypto/>

安全可能是一个难以驾驭的领域，随着竞争对手争夺地位和实现声誉稳健，索赔和反索赔满天飞。如果没有外部专家的帮助，消除噪音是不可能的，这就是为什么对安全产品进行专家审核是如此重要。

也就是说:加密信息应用 [Wire](https://web.archive.org/web/20230126231705/https://techcrunch.com/2015/04/29/wire-the-communications-app-backed-by-skypes-co-founder-arrives-on-the-web/) 现在[公布了对其加密协议 Proteus 的外部审计](https://web.archive.org/web/20230126231705/https://www.x41-dsec.de/reports/Kudelski-X41-Wire-Report-phase1-20170208.pdf)，以及该协议在其各种应用中的实现。

这是一项付费审计，由两名安全研究人员为 Wire 进行，他们是来自 [Kudelski Security](https://web.archive.org/web/20230126231705/https://www.kudelskisecurity.com/) 的 Jean-Philippe Aumasson 和来自 [X41 D-Sec](https://web.archive.org/web/20230126231705/https://www.x41-dsec.de/) 的 Markus Vervier。

在一篇详细介绍该审查的[中型文章](https://web.archive.org/web/20230126231705/https://medium.com/wire-news/wires-independent-security-review-61f37a1762a8#.w6loc4j15)中，Wire 写道:“该审查涵盖了 Proteus 在 Wire 可用的所有平台上的实现——iOS、Android、macOS、Windows、Linux 和 Wire for Web，可在现代的、支持 webRTC 的浏览器中工作。”

在这一点上，外部审计可能对 Wire 特别有价值，因为它最近在一篇通过 Twitter 分享并引起安全社区注意的[批评性博客帖子](https://web.archive.org/web/20230126231705/https://medium.com/@pepelephew/a-look-at-how-private-messengers-handle-key-changes-5fd4334b809a#.a4tbm9ycw)之后受到了一些抨击。

Wire 否认了这些批评，并争辩说,它受到了社交媒体上匿名账户的不公平攻击。TechCrunch 联系了最初那篇批评文章的作者，她在媒体上的名字是 [Tina Membe](https://web.archive.org/web/20230126231705/https://medium.com/@pepelephew?source=post_header_lockup) ，但此人不愿向我们透露他或她的身份——只是自称“不是真正的安全研究员”。

尽管如此，这位人士支持他们对 Wire 代码的批评，称其“非常混乱”，并特别批评了 Wire 执行证书锁定的方式——辩称他们的方法有缺陷，因为它可能被国家级攻击者绕过。

“举个例子，只有当证书的‘主题替换名’与 http://wire.com 匹配或者以 http://wire . com 结尾时，代码才会启用‘锁定’，”他们指着 Wire 代码的这一部分告诉我们。但是“主题替换名称”在证书中是可选的。攻击者将从任何 CA(中国、突尼西亚、土耳其等)发出一个 http://wire.com“普通名”的证书，省略“主题替换名”,这将认为它是有效的。

“我认为这是一个非常明显的错误，一个真正的安全研究员可以为你验证，”他们补充说。(在这次谈话之后，Membe 写了另一篇博客，详细描述了认证验证漏洞——可以在这里找到[。)](https://web.archive.org/web/20230126231705/https://medium.com/@pepelephew/wires-certificate-validation-vulnerability-f2b415298e2e#.jbk1gi7j2)

**更新:** Wire 表示已经在 1 月 27 日之前修复了 Membe 发现的证书锁定问题。“这个缺陷的范围非常有限，它只影响了 Android，它只影响了传输加密。“有线电视使用 Proteus 的端到端加密不受此影响，”Duric 说。他补充说，安全审查人员也被要求在部署之前检查修复方法。(关于修复的更多细节[请看这里](https://web.archive.org/web/20230126231705/https://github.com/wireapp/wire-android-sync-engine/pull/47)。部署补丁的代码部分可以在这里找到。)

Wire 的安全审查人员确实发现了该软件的一些其他问题，包括一个允许传输和处理无效公钥而不被标记为错误的漏洞。但审查人员也描述了被审查的组件具有“高度的安全性，这要归功于最先进的加密协议和算法，以及减轻软件错误风险的软件工程实践”。

该评论涵盖了 Wire 的协议规范和协议实现。更具体地说，它的 Proteus 消息协议和 Cryptobox API 及其 C 包装器 Cryptobox-C 的实现。“Cryptobox 为 Proteus 定义了一个简单的高级 API，以便在有线应用中向呼叫者隐藏协议的复杂性，”Wire 对该组件的解释是。

审查还包括 Proteus 和 cryptobox 的 CoffeeScript 对应物，如在 proteus.js 和 cryptobox.js 中实现的。

Wire 联合创始人兼首席技术官 Alan Duric 表示，第三层安全审查——全面考虑完整的解决方案——仍在进行中。

在审核概述中，外部安全审核人员写道:

> 由于采用了最先进的加密协议和算法以及降低软件缺陷风险的软件工程实践，经审查发现这些组件具有很高的安全性。尽管如此，还是发现了一些问题，其中一些问题可能会导致安全级别降低。所发现的问题在安全性方面都不严重。例如，我们发现可以传输和处理无效的公钥，而不会产生错误。结果，由通信方协商的共享秘密变得可预测，这反过来削弱了在“侵入恢复”方面的安全保证。此问题的根本原因是第三方组件中的错误(忽略验证错误代码)。我们建议修复此问题，并实施其他安全改进来解决线程不安全风险、内存中的敏感数据以及本报告中描述的其他方面。

Wire 表示，它已经修复了审查发现的所有问题，并在 iOS 和 Android 上部署了修复程序，并且正在为 web 及其桌面应用程序部署 Wire。

不言而喻，对于任何安全产品来说，不安全感都会造成真实而持久的损害。因此，Wire 显然希望对其加密技术的外部审查有助于消除它所招致的一些批评 Duric 很快向我们展示了一位安全学者对审计的早期评估样本:

“Kudelski 是独立审查员，”Duric 通过电子邮件补充说，该公司支付进行审计。“在该领域具有悠久传统的公司和完成审查的专家都是该领域的领先专家。”

Katriel Cohn-Gordon 是一群学术安全研究人员之一，他审计了 Signal Protocol(T1)，这是一个同名的 Signal encrypted messaging 应用程序的动力，他也对 Wire 的举动表示欢迎。他在给 TechCrunch 的一封电子邮件中写道，“很高兴看到像 Wire 这样的公司对自己的安全性保持透明。”。“(审计)似乎写得很好，电报的迅速回应是一个好迹象。”

值得注意的是，虽然 Signal 的协议与 Wire 的 Proteus 协议不同，但 Wire 确实使用了 Signal 协议的创建者 Open Whisper Systems 编写的一些开源组件，因此其 Proteus 协议代码显示了反映这种重用的版权归属。

Wire 成立于 2012 年，总部位于瑞士，由 Skype 联合创始人贾纳斯·弗里斯(Janus Friis)提供支持。虽然它开始时更多的是关注一般的通信，但后来它转移到将自己标榜为“关注隐私”的“私人信使”——在去年 3 月[日](https://web.archive.org/web/20230126231705/https://medium.com/@wireapp/hello-video-calls-hello-privacy-61a189aec23d#.5nk0rw4pq)将端到端加密扩展到其平台上的所有消息类型(不仅仅是通话)。

去年[12 月](https://web.archive.org/web/20230126231705/https://techcrunch.com/2016/12/16/encrypted-messaging-app-wire-adds-usernames-so-you-can-limit-what-you-share-with-contacts/)它还增加了用户名选项，这意味着注重隐私的用户不需要分享他们的电话号码或电子邮件来与其他有线用户交流。虽然这款应用仍然是免费的，但 T4 表示今年将推出付费服务。

它还表示，在继续开发应用程序的同时，承诺从现在开始定期进行外部安全审查。

“向前看，Wire 的每一项重大发展都将包括安全审查，”它写道。“我们将继续与 Kudelski Security 和 X41 D-Sec 等安全专家合作，共同完成完整的解决方案评估。

“所有的网络客户端代码都在 GitHub 上，服务器代码将于 2017 年年底在 Q1 开源。”