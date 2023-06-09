# 脸书为下一个 10 亿用户扩大委托账户回收 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/04/18/facebook-expands-delegated-account-recovery-in-a-play-for-the-next-billion-users/>

脸书正在扩展一种新的账户恢复工具，该工具于 1 月份首次亮相，允许 GitHub 等其他网站建立加密的账户恢复令牌，这些令牌由脸书存储。当用户丢失了他们的 GitHub 密码并被锁定帐户时，他从脸书向 GitHub 发送恢复令牌，证明他的身份。

这是一个巧妙的安全功能，对隐私专家来说很容易销售，但它也是脸书战略的重要组成部分，以确保下一个 10 亿互联网用户将他们的在线体验集中在脸书。

在今天的 [F8](https://web.archive.org/web/20221111170040/https://beta.techcrunch.com/tag/f8/) 开发者大会上，脸书发布了[SDK 和文档](https://web.archive.org/web/20221111170040/https://developers.facebook.com/docs/delegated-recovery/)，这将允许除 GitHub 之外的开发者为他们自己的测试用户设置委托账户恢复。一旦设置就绪，开发者可以申请脸书的测试程序，并开始向他们的用户提供该功能。

委托帐户恢复旨在使帐户恢复更加安全。如果你曾经忘记过密码(谁没有呢？)您知道，恢复过程通常包括发送到您电子邮件的链接或发送到您手机的安全码。但是，如果用户的密码被列入数据泄露，或者他们中了网络钓鱼的圈套，电子邮件就很容易受到威胁，如果你升级到新手机或更换号码，短信安全码可能会在传输中丢失。

“该系统被设计为即使对于已经变得太常见的电子邮件和用户数据库的大规模数据转储也具有弹性。脸书安全工程师 Brad Hill 在一篇博客文章中解释说:“恢复令牌需要独立持有的密钥才能使用，因此它提供了一种我们在电子邮件中看不到的安全级别。以下是恢复流程的工作方式:

![](img/a714f38f0e12a12435eaa453947ff12e.png)

但是，即使最高级别的帐户安全性对一些用户来说不是卖点，Hill 在 1 月[日](https://web.archive.org/web/20221111170040/https://beta.techcrunch.com/2017/01/30/facebook-challenges-email-for-control-of-your-online-identity/)首次推出委托帐户恢复功能时，也给了我一个简洁而有说服力的理由来解释为什么委托帐户恢复比其他方法更好:“即使你把手机丢下船，我们也能让你回到你的帐户。”

脸书与 GitHub 一起推出了这项功能，GitHub 的用户更倾向于技术，可以更容易地浏览设置过程。现在，脸书正在将委托账户恢复扩展到其他网站，它需要说服开发者，额外的设置障碍——以及与脸书的联系——值得从电子邮件转向其他网站。

一些在线零售商可能会很快采用委托账户恢复，但很容易想象亚马逊、谷歌或 Twitter 会抵制这一想法。这也是该项目开源的部分原因:其他公司也可以把自己打造成身份中心。“消除欺诈是一个共同的目标，而不是一个竞争空间，”希尔说。“拥有多个供应商将有助于这个生态系统。”如果生态系统增长，安全性也会扩大。用户可以在几个不同的站点存储加密数据的恢复令牌，因此用户需要证明可以访问多个帐户才能解密数据。

让其他公司参与进来，无论是通过向脸书存放恢复令牌，还是自己发行令牌，都将有助于脸书在美国和欧洲以外的地区发展，在这些地区，电子邮件恢复已经很少见了。

“脸书用户调查显示，使用个人电子邮件的人在减少，而越来越喜欢用电话号码来识别账户。Hill 解释说:“在非洲和亚太地区的一些地方，相比电子邮件，对电话号码的偏好高达 70%。“在许多电话号码最受欢迎的地方，它也是一个非常不稳定的标识符。人们经常拥有多张 sim 卡，频繁更换号码以获得更好的交易，并将电话号码视为垃圾邮件收集账户，就像英语市场中的人们经常处理电子邮件一样。”

由于这些市场的用户正放弃电子邮件，转而将电话号码作为他们的主要身份枢纽，脸书需要跟随这一趋势。将自己树立为用户在线身份的主要持有者，让脸书得以延续，即使其用户放弃 SIM 卡或更改电子邮件地址。就像脸书的 Internet.org 项目一样，授权账户恢复可以让脸书成为下一个十亿用户在线体验的基础部分。

“如果你依赖电子邮件来恢复，你将会错过与很多人交流的机会。而且，如果你用一个电话号码让人们注册你的服务，当号码改变时，你有办法恢复是很重要的，”希尔补充道。

如果脸书能够鼓励广泛采用委托账户恢复，这将是脸书内外用户安全的胜利，也是该公司扩张计划的胜利。现在这个特性对 GitHub 之外的开发者开放了，我们将会看到它会被多广泛地采用。