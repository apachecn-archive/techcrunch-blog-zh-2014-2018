# WPA2 显示易受关键重新安装攻击

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/10/16/wpa2-shown-to-be-vulnerable-to-key-reinstallation-attacks/>

今天 WPA2 wi-fi 协议中的一个关键重新安装攻击漏洞[被公之于众。安全研究员](https://web.archive.org/web/20230316161113/https://www.krackattacks.com/) [Mathy Vanhoef](https://web.archive.org/web/20230316161113/http://www.mathyvanhoef.com/) 发现了他所谓的无线协议中的“严重弱点”。

TL；灾难恢复是在登录到无线网络的人的范围内，攻击者可以使用密钥重新安装攻击来绕过 WPA2 网络安全，读取以前被认为是安全加密的信息，从而使他们能够窃取通过网络传输的敏感数据，如密码、信用卡号、聊天消息、电子邮件、照片等。

“这种攻击针对所有现代受保护的无线网络，”范霍夫说。

他说，根据网络配置，该漏洞还允许攻击者注入和操纵数据——例如，通过向网站添加勒索软件或恶意软件。

以下是他的[研究论文](https://web.archive.org/web/20230316161113/https://papers.mathyvanhoef.com/ccs2017.pdf)摘要中的相关段落:

> 所有受保护的 Wi-Fi 网络都使用 4 次握手来生成新的会话密钥。到目前为止，这个 14 年的握手仍然没有受到攻击，甚至被证明是安全的。然而，我们表明 4 次握手易受密钥重新安装攻击。在这里，对手诱骗受害者重新安装一个已经在使用的密钥。这是通过操纵和重放握手消息来实现的。当重新安装密钥时，相关的参数，例如递增的发送包号(nonce)和接收包号(replay counter)被重置为它们的初始值。我们的密钥重新安装攻击还会破坏 PeerKey、组密钥和快速 BSS 转换(FT)握手。影响取决于被攻击的握手和使用的数据保密协议。简而言之，针对 AES-CCMP，对手可以重放和解密(但不能伪造)数据包。这使得劫持 TCP 流并向其中注入恶意数据成为可能。对 WPATKIP 和 GCMP 的影响是灾难性的:数据包可以被重放、解密和伪造。因为 GCMP 在两个通信方向上使用相同的身份验证密钥，所以受到的影响尤其大。

“弱点在于 Wi-Fi 标准本身，而不在于个别产品或实施。因此，任何对 WPA2 的正确实施都可能受到影响，”他进一步写道。“为了防止攻击，用户必须在安全更新可用时立即更新受影响的产品。

“请注意，如果您的设备支持 Wi-Fi，它很可能会受到影响。在我们最初的研究中，我们发现 Android、Linux、Apple、Windows、OpenBSD、MediaTek、Linksys 等都受到了某种形式的攻击的影响。有关特定产品的更多信息，请咨询 CERT/CC 的[数据库，或联系您的供应商。”](https://web.archive.org/web/20230316161113/https://www.kb.cert.org/vuls/byvendor?searchview&Query=FIELD+Reference=228519&SearchOrder=4)

在研究论文中，他将此次攻击描述为对 Android 6.0 的“异常毁灭性”的攻击。

“由于安卓使用 wpa_supplicant，安卓 6.0 及以上版本也包含该漏洞。这使得拦截和操纵这些 Linux 和 Android 设备发送的流量变得轻而易举，”他在 [Krackattacks](https://web.archive.org/web/20230316161113/https://www.krackattacks.com/) 网站上解释这一缺陷时写道。“请注意，目前 [41%的 Android 设备](https://web.archive.org/web/20230316161113/https://developer.android.com/about/dashboards/index.html)容易受到我们攻击的这种异常破坏性的变种的攻击。”

他进一步写道，虽然论文中详细描述的一些攻击可能看起来很难实现，但后续工作表明，针对 macOS 和 OpenBSD 的攻击“更加普遍，也更容易执行”，他补充道:“因此，尽管我们同意论文中的一些攻击场景相当不切实际，但不要让这一点欺骗你，让你相信关键的重新安装攻击在实践中不会被滥用。”

(虽然 OpenBSD 已经发布了一个补丁，但在 7 月份，在 Vanhoef 公开披露这一漏洞之前，他已经获悉了这一漏洞。)

范霍夫进一步展示了这种攻击如何仍然能够对使用 HTTPS 的网站和应用程序起作用，展示了这种增加的加密层如何能够在他描述为“令人担忧的许多情况下”被绕过(他标记了 HTTPS 被绕过的多个先前的例子)，在[非浏览器软件](https://web.archive.org/web/20230316161113/https://pdfs.semanticscholar.org/48fc/8f1aa0b6d1e4266b8017820ff8770fb67b6f.pdf)，在[苹果的 iOS 和 OS X](https://web.archive.org/web/20230316161113/https://www.imperialviolet.org/2014/02/22/applebug.html) ，在[安卓应用程序](https://web.archive.org/web/20230316161113/https://arstechnica.com/information-technology/2015/04/android-apps-still-suffer-game-over-https-defects-7-months-later/)，在[安卓应用程序](https://web.archive.org/web/20230316161113/https://arxiv.org/ftp/arxiv/papers/1505/1505.00589.pdf)，在[银行应用程序](https://web.archive.org/web/20230316161113/http://blog.ioactive.com/2014/01/personal-banking-apps-leak-info-through.html)，甚至在 [VPN 应用程序](https://web.archive.org/web/20230316161113/https://arstechnica.com/information-technology/2017/01/majority-of-android-vpns-cant-be-trusted-to-make-users-more-secure/))

他还制作了下面的视频演示，展示了中间人技术在 Android 和 Linux 上工作，以 Match.com 的一个虚拟用户作为样本目标，以明文形式获取他们的用户名和密码。

范霍夫将在 11 月 1 日举行的[计算机和通信安全(CCS)](https://web.archive.org/web/20230316161113/https://acmccs.github.io/session-F3/) 会议上展示这项研究。

他的研究论文题为[密钥重新安装攻击:在 WPA2 强制随机数重用](https://web.archive.org/web/20230316161113/https://papers.mathyvanhoef.com/ccs2017.pdf)。

在一份关于攻击的声明中， [Wi-Fi Alliance](https://web.archive.org/web/20230316161113/https://www.wi-fi.org/news-events/newsroom/wi-fi-alliance-security-update) 敦促无线设备的用户总是为他们的所有设备安装最新的软件更新，并指出“主要平台提供商”已经开始部署针对特定 WPA2 漏洞的补丁(补丁需要确保一个密钥只安装一次——这可以防止攻击)。

目前还不清楚所有 wi-fi 设备打补丁以及它们的用户更新以获得安全补丁需要多长时间，但不可避免的是，一些无线设备和一些无线用户在一段时间内仍然容易受到这种攻击。

“一旦有安全更新，就更新你所有的设备，”范霍夫建议道。

他还敦促更新你的 wi-fi 路由器的固件。并警告不要为了防范 WPA2 的攻击而暂时切换到 WEP——考虑到 WEP 的无数和有据可查的漏洞仍然意味着它更糟糕。

以下是完整的 Wi-Fi 联盟声明:

> 最近发表的研究发现了一些 Wi-Fi 设备中的漏洞，这些设备在特定条件下会重新安装网络加密密钥，从而禁用重播保护并显著降低加密的安全性。这个问题可以通过简单的软件更新来解决，包括主要平台提供商在内的 Wi-Fi 行业已经开始向 Wi-Fi 用户部署补丁。用户可以期待他们所有的 Wi-Fi 设备，无论是打补丁的还是没打补丁的，都能继续很好地协同工作。
> 
> 没有证据表明该漏洞被恶意利用，Wi-Fi Alliance 已立即采取措施，确保用户可以继续依靠 Wi-Fi 提供强大的安全保护。Wi-Fi Alliance 现在要求在我们的全球认证实验室网络中测试该漏洞，并提供了一个漏洞检测工具供任何 Wi-Fi Alliance 成员使用。Wi-Fi Alliance 还向设备供应商广泛传达了有关该漏洞的详细信息和补救措施，并鼓励他们与解决方案提供商合作，快速集成任何必要的补丁。和往常一样，Wi-Fi 用户应该确保他们已经安装了设备制造商推荐的最新更新。
> 
> 与任何技术一样，先发制人地识别潜在漏洞的强大安全研究对于保持强有力的保护至关重要。Wi-Fi 联盟感谢[鲁汶大学 imec-DistriNet 研究小组的 Mathy Vanhoef](https://web.archive.org/web/20230316161113/http://www.mathyvanhoef.com/) 和 Frank Piessens 发现并负责任地报告了这个问题，使行业能够主动准备更新。Wi-Fi Alliance 还感谢 Mathy Vanhoef 在协调响应期间提供的支持，特别是他对漏洞检测工具的贡献。
> 
> 更多信息，请参考来自 [ICASI](https://web.archive.org/web/20230316161113/https://www.icasi.org/) 和 [CERT](https://web.archive.org/web/20230316161113/https://cert.org/) 的声明。