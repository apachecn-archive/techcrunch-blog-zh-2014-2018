# 苹果正在修复导致点击链接导致 iPhones 崩溃的 iOS 漏洞 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/03/28/its-not-just-you-clicking-on-links-in-ios-9-3-can-crash-your-iphone/>

七轮测试版是不够的——许多 iOS 用户在苹果支持论坛上报告[一个 bug 正在影响他们的设备。当他们点击 Safari、Chrome、Mail、Messages、Notes 和其他应用程序中的链接时，应用程序会冻结并崩溃。如果你是其中之一，这里有一个补丁可以解决你的问题。](https://web.archive.org/web/20221007060903/https://discussions.apple.com/thread/7505840)

**更新:**苹果公司表示，他们正在对该问题进行软件修复:

> 我们知道这个问题，我们将很快在软件更新中发布修复程序。

看起来这个问题与通用链接有关。随着 [iOS 9](https://web.archive.org/web/20221007060903/https://beta.techcrunch.com/2015/09/16/ios-9-review/) ，苹果推出了[通用链接](https://web.archive.org/web/20221007060903/https://developer.apple.com/library/ios/documentation/General/Conceptual/AppSearch/UniversalLinks.html)，这是一种全新的处理本地应用链接的方式。YouTube 等应用开发者可以注册域名，绕过 Safari，直接在应用中打开网页链接。

这就是为什么当你点击一个`youtube.com/somethingsomething`链接时，iOS 会打开 YouTube 应用，而不是在 Safari 中加载网页。这是一个很棒的功能，除非应用开发者滥用它。

Sergey Roshchin [发布了一个视频](https://web.archive.org/web/20221007060903/https://www.youtube.com/watch?v=OaR_wWcKfMs)展示了今天的 bug。他的 iPad 运行良好。但后来，他安装了 Booking.com 应用程序，Safari 就无法使用了。当他点击一个链接时，它会挂起，然后崩溃。

Booking.com 将其应用与各种各样的领域联系在一起——准确地说，领域太多了。由于有 2.4MB 的域名深层链接条目，当 iOS 根据其通用链接数据库检查链接时，Safari 和其他应用程序会崩溃，因为该数据库太大了。一位消息人士还告诉我，iOS 9.3 中的[航海家-SNCF](https://web.archive.org/web/20221007060903/http://www.voyages-sncf.com/) 应用程序也会崩溃。**更新:**航次-SNCF [没有通用链接](https://web.archive.org/web/20221007060903/https://twitter.com/rosyna/status/714442380368175104)，所以这个应用应该不会引起任何问题。

然而，Booking.com 的应用程序在 3 月 17 日更新，在 iOS 9.3 发布之前。可以肯定的是，在处理这些链接时，iOS 9.3 发生了一些变化，导致了应用程序崩溃。

[WebKit 团队](https://web.archive.org/web/20221007060903/https://twitter.com/webkit)发布了一个[巨大的更新](https://web.archive.org/web/20221007060903/https://developer.apple.com/library/mac/releasenotes/General/WhatsNewInSafari/Articles/Safari_9_1.html)iOS 9.3 和 OS X 10.11.4。Safari 9.1 包含了许多变化。也许通用链接错误与这个 WebKit 更新有关，也许没有。

不管怎样，如果你遇到这个错误，苹果可能会在下一次错误修复更新中修复它。与此同时，你应该删除 Booking.com 应用程序，然后…等等。它不会立即修复你的问题，因为 iOS 会不时地检查通用链接。但至少，你的 iPhone 明天又能用了。

**更新:**删除 Booking 的应用可能还不够。

![Screen Shot 2016-03-28 at 2.26.04 PM](img/2a5090d0133bc17faffadee0e3eb2424.png)

更新:Booking.com 发给我以下声明:

> 我们已经发现了通用链接框架的一些问题，这似乎是苹果 iOS 9.3 特有的问题。我们知道他们正在改正，我们会尽我们所能帮助他们尽快解决问题。