# 这个新的文本炸弹用一个单一的 Unicode 符号崩溃了大多数 Mac 和 iOS 应用程序

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/15/iphone-text-bomb-ios-mac-crash-apple/>

# 这个新的文本炸弹用一个单一的 Unicode 符号崩溃了大多数 Mac 和 iOS 应用程序

TechCrunch 获悉，一个潜在的严重新漏洞影响了大量苹果设备。

在他们开发国际新闻源的过程中，Aloha Browser 的软件工程师发现了两个非英语语言的 Unicode 符号，这两个符号可以让任何使用苹果默认旧金山字体的苹果设备崩溃。该漏洞导致 iPhones、iPads、MAC 甚至手表操作系统设备崩溃，这些设备在屏幕上显示包含该符号的文本。

当两个符号中的一个显示在应用程序中时，该软件会立即崩溃。在许多情况下，应用程序无法重新打开，必须重新安装。TechCrunch 能够在两台运行旧版本 iOS 的 iPhone、一台运行 iOS 11.2.5 的 iPhone 和一台运行 High Sierra 的 MacBook Pro 上重现这种行为。

该漏洞导致包括邮件、推特、信息、Slack、Instagram 和脸书在内的应用崩溃。根据我们的测试，它还崩溃了 Jumpcut，一个用于 Mac 的复制粘贴插件。虽然最初 Mac 版 Chrome 浏览器似乎没有受到影响，可以安全地显示该符号，但后来它使 Chrome 崩溃，该软件在卸载并重新安装之前不会重新打开。

TechCrunch 一直在与苹果公司就软件修复的潜在时间表进行接触，并将相应地更新这个故事。据 Aloha Browser 的团队称，苹果公司已经意识到了这个漏洞，而且另一个开发团队也可能已经报告了这个问题。【**更新:**苹果公司已经确认即将推出补丁。显然，这只会影响软件的当前版本，这一问题已经在 iOS、tvOS、macOS 和 watchOS 的测试版中得到解决。]

这是苹果今年第二个令人头疼的短信炸弹。今年 1 月，软件研究人员亚伯拉罕·马斯里发现了一个 [iOS 的小故障](https://web.archive.org/web/20230324125435/https://techcrunch.com/2018/01/23/the-latest-ios-update-fixes-a-glitch-that-would-let-others-crash-your-phone-with-a-text-message/)，这个小故障允许一个特定的网址让任何收到短信的 iPhone 崩溃，有时会导致内核崩溃。在 2016 年，如果用户点击 CrashSafari.com 的网址，另一个错误可能会使任何 iPhone 或 Safari 浏览器崩溃。2015 年，一种所谓的“[死亡 Unicode](https://web.archive.org/web/20230324125435/https://www.cultofmac.com/324043/apple-confirms-imessage-bug-is-crashing-iphones/)”可能会使用一些阿拉伯字符使 iPhone 的内存过载。现在我们看到的是死亡 Unicode 2.0。

由于如此多的应用程序受到影响，如果通过开放的社交平台发送垃圾邮件或通过电子邮件或短信针对个人，新的文本炸弹可能会被用来制造大规模混乱。这个新漏洞影响了大量苹果设备，并使它们运行的几乎所有主要应用程序崩溃，如果不迅速解决，它的破坏性尤其大。