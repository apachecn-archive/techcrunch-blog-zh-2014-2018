# 苹果将在 2016 年底要求 iOS 应用程序使用 HTTPS 连接

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/06/14/apple-will-require-https-connections-for-ios-apps-by-the-end-of-2016/>

# 到 2016 年底，苹果将要求 iOS 应用程序使用 HTTPS 连接

在苹果[全球开发者大会](https://web.archive.org/web/20230225042954/https://techcrunch.com/tag/wwdc2016/)的一次安全演示中，该公司透露了其应用商店中所有应用开启一项名为 App Transport Security 的重要安全功能的截止日期——2017 年 1 月 1 日。

“今天，我很自豪地说，在 2016 年底，应用传输安全正在成为应用商店应用的一项要求，”苹果安全工程和架构负责人伊万·克尔斯蒂奇在 WWDC 的一次演讲中说。“这将为我们的用户和您的应用程序在网络上的通信提供大量真正的安全性。”

App Transport Security，简称 ATS，是苹果在 iOS 9 中首次亮相的一项功能。当 ATS 启用时，它会强制应用程序通过 HTTPS 连接而不是 HTTP 连接到 web 服务，从而通过加密保护用户数据在传输过程中的安全。

HTTPS 语中的“S”代表安全，当你登录银行或电子邮件账户时，你会经常看到它出现在你的浏览器中。但移动应用通常对用户的网络连接安全性并不透明，而且很难判断一个应用是通过 HTTP 还是 HTTPS 连接的。

输入 ATS，iOS 9 默认启用 ATS。然而，开发者仍然可以关闭 ATS，允许他们的应用程序通过 HTTP 连接发送数据——直到今年年底。(对于技术人群:ATS 需要 TLS v 1.2，已经加密的批量数据除外，如媒体流。)

2016 年底，苹果将对所有希望向 App Store 提交应用的开发者强制执行 ATS。一直在[考虑](https://web.archive.org/web/20230225042954/https://forums.developer.apple.com/thread/47544)何时会对 HTTP 下手的应用程序开发人员现在可以松一口气了，因为他们有了一个明确的截止日期，用户也可以放松了，因为他们知道他们 iPhones 和 iPads 上的所有应用程序都将强制安全连接。

通过要求开发者使用 HTTPS，苹果加入了一个更大的保护数据在线传输的运动。虽然安全协议在登录页面上很常见，但许多网站仍然使用普通的老式 HTTP 进行大多数连接。随着许多网站艰难地过渡到 HTTPS，这种情况正在慢慢改变(《连线》杂志特别擅长[记录这个过程](https://web.archive.org/web/20230225042954/http://www.niemanlab.org/2016/04/wireds-making-the-long-and-slow-switch-to-https-and-it-wants-to-help-other-news-sites-do-the-same/))。