# 与我私下交谈:iPhone TechCrunch 的免费全球加密语音通话信号

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/07/29/talk-private-to-me-free-worldwide-encrypted-voice-calls-with-signal/>

# 跟我说悄悄话:免费的、全球范围的、带 iPhone 信号的加密语音通话

快乐吧，隐私的爱好者们！因为[Open whispers systems](https://web.archive.org/web/20230130100805/https://whispersystems.org/blog/signal/)已经发布了用于 iPhone 的[信号，这给了任何一个 iPhone 用户完全加密他们的通话以防止窃听的权力——并且完全兼容 OWS 久经考验并广受欢迎的用于 Android](https://web.archive.org/web/20230130100805/http://itunes.apple.com/app/id874139669) 的 [RedPhone。](https://web.archive.org/web/20230130100805/https://play.google.com/store/apps/details?id=org.thoughtcrime.redphone)

在引擎盖下，Signal 使用推送通知来发起呼叫，亚马逊网络服务来路由数据，以及由 [Phil Zimmerman](https://web.archive.org/web/20230130100805/http://en.wikipedia.org/wiki/Phil_Zimmermann) 开发的 [ZRTP](https://web.archive.org/web/20230130100805/http://tools.ietf.org/html/rfc6189) 协议来加密端到端的对话。你不需要新密码或新号码；它是专为工作而设计的 ^(TM) 。哦，你的呼叫的元数据也被保护/丢弃。

代码是[开源的](https://web.archive.org/web/20230130100805/https://github.com/WhisperSystems/Signal-iOS)，并且有一个[有趣的贡献者资助模型](https://web.archive.org/web/20230130100805/https://whispersystems.org/blog/bithub/)；每一个合并的拉取请求都会得到一部分比特币的回报，作为一个整体捐赠给这个项目。

Open WhisperSystems iOS 团队——安全研究员 [Frederic Jacobs](https://web.archive.org/web/20230130100805/https://twitter.com/FredericJacobs) 和天体物理学家/黑客/工程师 [Christine Corbett](https://web.archive.org/web/20230130100805/https://twitter.com/corbett) (免责声明/披露；Christine 的一个朋友)——他们也在开发与 OWS 的 Android 版 TextSecure 兼容的加密文本通信，并有望在今年夏天晚些时候作为新版 Signal 的一部分发布。届时，在 Android 方面，RedPhone 和 TextSecure 将类似地整合为一个统一的 Android 信号应用程序。浏览器扩展的开发也在进行中，这样你就可以在电脑上安全地打电话了。

ZRTP 反监视武器库的一个怪癖是:为了防范[中间人攻击](https://web.archive.org/web/20230130100805/http://en.wikipedia.org/wiki/Man-in-the-middle_attack)，它为每个对话随机生成一对词——上面截图中的“曲棍球出版商”。用户可以通过简单地相互背诵来确保他们的单词对匹配。[如果不符合](https://web.archive.org/web/20230130100805/http://zfoneproject.com/faq.html#mitm)，那就是中间有男人的标志。

对于开放语者系统来说，这是一个忙碌的夏天。一个月前，他们从骑士基金会获得了[416，000 美元的资助，上周他们](https://web.archive.org/web/20230130100805/http://www.knightfoundation.org/grants/201499909/)[还发布了 Flock](https://web.archive.org/web/20230130100805/https://whispersystems.org/blog/flock/) ，这是一个私有的——当然，也是高度安全的 Android 日历和联系人的云同步服务。