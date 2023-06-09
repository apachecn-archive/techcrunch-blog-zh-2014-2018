# Western Digital My Cloud drives 中的密码旁路漏洞使数据面临风险

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/19/password-bypass-flaw-western-digital-my-cloud-drives/>

# Western Digital My Cloud drives 中的密码绕过漏洞将数据置于风险之中

一名安全研究人员公布了一个受欢迎的云存储驱动器中的漏洞的细节，此前该公司一年多来未能发布安全补丁。

雷姆科·维穆伦在西部数据公司的“我的云设备”中发现了[一个权限升级漏洞](https://web.archive.org/web/20230404191101/https://www.securify.nl/advisory/SFY20180102/authentication-bypass-vulnerability-in-western-digital-my-cloud-allows-escalation-to-admin-privileges.html)，他说这使得攻击者能够绕过硬盘上的管理员密码，获得对用户数据的“完全控制”。

这种利用之所以有效，是因为 drive 基于 web 的仪表板在授予潜在攻击者访问需要更高级别访问权限的工具之前，没有正确检查用户的凭据。

维穆伦在一封电子邮件中告诉 TechCrunch，这个漏洞“很容易”被利用，如果我的云设备允许通过互联网远程访问，就可以被远程利用——T4 成千上万的设备都这样做。他在 Twitter 上发布了一个概念验证视频。

该漏洞的细节也被另一个安全团队独立发现[，该团队发布了](https://web.archive.org/web/20230404191101/https://twitter.com/Exploiteers/status/1042093284666040325)[自己的漏洞利用代码](https://web.archive.org/web/20230404191101/https://pastecry.pt/dUHB3e#PewMuk%3AUt2Ek3Bee4Rej2Syz5Mek)。

一年多前，即 2017 年 4 月，维穆伦报告了这个漏洞，但表示该公司停止了回应。通常情况下，安全研究人员会给公司 90 天的时间做出回应，这符合行业公认的负责任的披露准则。

在他发现 WD 同时更新了 My Cloud 固件，但没有修复他发现的漏洞后，他决定发布他的发现。

一年过去了，WD 依然没有发布补丁。

该公司证实，它知道这个漏洞，但没有说明为什么花了一年多的时间来发布补丁。“我们正在完成一个预定的固件更新，将解决报告的问题，”一位发言人说，这将在“几周内”到来

WD 表示，它的几款 My Cloud 产品容易受到攻击，包括 EX2、EX4 和 Mirror，但不包括 My Cloud Home。

与此同时，维穆伦表示，目前还没有解决方案，如果用户想保证数据安全，他们必须“直接断开”硬盘。