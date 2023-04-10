# 苹果关闭了首个全功能 Mac OS X 勒索软件 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/03/07/apple-has-shut-down-the-first-fully-functional-mac-os-x-ransomware/>

苹果已经关闭了第一个针对 Mac 电脑的全功能勒索软件。这种特殊形式的网络威胁包括恶意软件，它会加密你个人电脑上的数据，使你无法再访问这些数据。之后，黑客要求你用一种难以追踪的数字货币——在这里是比特币——支付给他们，这样你就可以取回你的文件。这个名为 KeRanger 的勒索软件是由帕洛阿尔托网络公司的研究人员首次报道的。他们还指出，苹果现在已经撤销了攻击中使用的滥用证书，并用新的签名更新了内置的反恶意软件系统 XProtect，以保护客户。

从技术上讲，KeRanger 并不是第一个针对 Mac 用户的勒索软件。这家安全公司表示，之前已经发现了另一个名为 [FileCoder](https://web.archive.org/web/20230127141259/https://securelist.com/blog/research/66760/unfinished-ransomware-for-macos-x/) 的恶意软件应用。然而，FileCoder 在被发现时是不完整的，这就是为什么该公司认为 KeRanger 是第一个出现在 OS X 平台上的功能性勒索软件。

OS X 现在成为攻击目标的事实表明了苹果操作系统的受欢迎程度——勒索软件是当今一种相当常见的网络威胁形式，因为受害者往往很可能屈服于攻击者的要求。甚至在一些高调的攻击中也出现了这种情况，比如上个月关闭洛杉矶一家医院服务器的[勒索软件。医院最终支付了相当于 17，000 美元的比特币来恢复系统的运行。](https://web.archive.org/web/20230127141259/https://techcrunch.com/2016/02/17/la-hospital-servers-shut-down-by-ransomware/)

对于 KeRanger，需求更加温和，尽管目前还不清楚有多少用户实际上成为了攻击的受害者，以及它在利用这些受害者方面有多成功。

值得一提的是，帕洛阿尔托网络公司的威胁情报总监瑞安·奥尔森告诉我们，他的公司认为他们的快速行动加上苹果公司的快速反应“极大地限制了这种威胁的影响。”

根据 Palo Alto Networks 的说法，攻击者用恶意软件感染了开源 BitTorrent 客户端 [Transmission](https://web.archive.org/web/20230127141259/https://www.transmissionbt.com/) 的两名安装人员，该恶意软件随后会加密文件，然后要求一个比特币(约 400 美元)的赎金，以将文件释放回用户的控制。

![fig7-500x236](img/3aa75501d66a24beced5d5540774ddd4.png)

![fig8-500x161](img/729a0254c149ae5dc9206bca0aa5d5b0.png)

KeRanger 应用程序本身签署了有效的 Mac 应用程序开发证书，这就是它如何能够绕过苹果的看门人保护机制。Palo Alto Networks 表示，在 3 月 4 日接到威胁警报后，苹果公司本周末迅速采取行动，撤销了该证书，并更新了防病毒签名。

苹果公司目前尚未公布关于 KeRanger 的详细移除或支持信息，但该公司向 TechCrunch 证实，证书已被撤销，因此没有人可以安装受影响的应用程序。我们知道，消费者保护自己的最佳方式是通过 [XProtect](https://web.archive.org/web/20230127141259/http://www.howtogeek.com/217043/xprotect-explained-how-your-macs-built-in-anti-malware-works/) 更新苹果的恶意软件档案。

终端用户也在[报告](https://web.archive.org/web/20230127141259/https://forums.developer.apple.com/thread/40476)看到保护“威胁”。恶意软件”在最新的 XProtect 更新中推出。苹果论坛上的其他用户对用户的建议有助于详细说明那些已经被恶意软件感染的人应该采取的步骤，这需要找到并删除某些隐藏文件。

[Transmission](https://web.archive.org/web/20230127141259/https://www.transmissionbt.com/) 也以自己的方式成为攻击的受害者，它也更新了网站，建议下载了受感染的 2.90 版本软件的用户升级并运行 2.92 版本。此版本将从系统中删除受恶意软件感染的文件。(Transmission 从未托管在 Mac App Store 上，但它的应用程序有自动更新机制，这将帮助那些没有手动升级的人。)

![Screen Shot 2016-03-07 at 10.35.22 AM](img/0fe5f83b67c5917694578a99d22b31d0.png)

此外，如果用户现在试图运行受感染版本的 Transmission，他们将会看到一个警告对话框，通知他们弹出磁盘映像，该应用程序将会损坏您的电脑，应该被移到废纸篓。

![fig13-500x220](img/5da5b5e41dce25d2a5e8c6adadbcb912.png)

虽然苹果已经解决了 KeRanger 带来的直接威胁，但鉴于该安全公司认为这种恶意软件仍在开发中，仍有一些担忧。它的分析表明，攻击者可能试图开发后门功能，加密用户的时间机器备份。

如果是这样的话，那么受害者将无法使用时间机器恢复他们的文件——他们将更容易受到黑客要求的摆布。