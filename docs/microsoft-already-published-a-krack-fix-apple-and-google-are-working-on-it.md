# 微软已经发布了一个补丁，苹果和谷歌正在努力

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/10/17/microsoft-already-published-a-krack-fix-apple-and-google-are-working-on-it/>

安全研究人员 Mathy Vanhoef 昨天公开披露了 WPA2 加密协议中的一个严重漏洞，该漏洞会影响所有使用 WiFi 的设备。虽然我们已经列出了[许多保护自己免受黑客攻击的方法](https://web.archive.org/web/20230118055212/https://techcrunch.com/2017/10/16/heres-what-you-can-do-to-protect-yourself-from-the-krack-wifi-vulnerability/)，但从你的网络中彻底根除它的最好方法是更新你所有的 WiFi 设备。一些公司比其他公司更快。

首先，你应该更新你的 WiFi 接入点。如果你使用的是默认的 ISP 路由器，你对此无能为力。询问该公司是否对其进行了修补，查找用户指南以了解如何访问配置面板并强制更新。

如果你担心，你也可以买一个单独的 WiFi 接入点，插在你的路由器上，禁用你路由器上的 WiFi。欧文·威廉姆斯一直做得很好[跟踪所有各种更新的状态](https://web.archive.org/web/20230118055212/https://char.gd/blog/2017/wifi-has-been-broken-heres-the-companies-that-have-already-fixed-it)，即使你有一个来自未知供应商的接入点。Ubiquiti、Microtik、Meraki、Aruba 和 FortiNet 立即更新了各自的固件。

但是更新你的接入点是不够的。您还需要更新您的设备。否则，如果你连接到一个未打补丁的未知 WiFi 网络，有人仍然可以查看你未加密的互联网流量，并收集一些关于你的个人数据。

所以让我们看看设备制造商。微软在这方面领先。The Verge [首先报道了](https://web.archive.org/web/20230118055212/https://www.theverge.com/2017/10/16/16481818/wi-fi-attack-response-security-patches)微软已经发布了[针对 Windows 7、Windows 8、Windows 8.1 和 Windows 10 的安全补丁](https://web.archive.org/web/20230118055212/https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2017-13080)。

据 iMore [报道](https://web.archive.org/web/20230118055212/https://www.imore.com/krack-wpa2-wi-fi-exploit-already-fixed-ios-macos-tvos-watchos-betas)，苹果也有锦囊妙计。不幸的是，该公司将等到下一个大版本来分享修复。所以这意味着你已经可以通过下载 macOS，iOS，tvOS 和 watchOS 的测试版来修复 KRACK 漏洞了。否则，苹果将在未来几周发布 macOS 10.13.1 和 iOS 11.1，并修复其他错误，推出新的表情符号等。

**更新:**苹果发言人发给我以下声明:

> “苹果坚定地致力于保护我们客户的数据。对 KRACK WiFi 漏洞的修复目前正在 iOS、macOS、watchOS 和 tvOS 的测试版中，并将很快向客户推出。"

但是安卓设备呢？这就是它变得乏味的地方。运行 Android 6.0 及更高版本的设备比其他设备更容易受到攻击。由于 WiFi 堆栈中握手机制的糟糕实现，很容易执行密钥重新安装攻击。

谷歌表示，11 月 6 日的补丁将解决这个问题。谷歌自己的设备将立即收到更新，但设备制造商和运营商批准更新还需要一段时间。事实上，这可能需要几周或几个月。Android 碎片在这些情况下并不理想。

但有一件事是肯定的。KRACK 漏洞证明您应该在安全更新可用时立即安装它们。打开设备上的自动更新，如果设备提示您安装补丁程序，请单击是。