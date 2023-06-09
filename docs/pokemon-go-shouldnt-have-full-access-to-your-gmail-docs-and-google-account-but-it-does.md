# Pokémon Go 不应该完全访问你的 Gmail、Docs 和 Google 账户，但它可以

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/07/11/pokemon-go-shouldnt-have-full-access-to-your-gmail-docs-and-google-account-but-it-does/>

当你使用谷歌登录 Pokémon Go 时，正如你们中的许多人已经做过的那样，这款受欢迎的游戏出于某种原因授予自己(至少对一些 iOS 用户来说)对你的谷歌帐户的最高访问权限，这意味着它可以读取你的电子邮件、位置历史记录……几乎所有内容。它为什么需要这个，为什么不告诉用户？[更新:[该公司现在表示正在修复这个漏洞](https://web.archive.org/web/20230404114230/https://techcrunch.com/2016/07/12/pokemon-go-promises-to-fix-the-bug-that-let-it-access-all-your-google-data/)，并且从未访问过用户谷歌账户信息之外的任何东西。

这是在发布后不久发现的，当时 [RedOwl 的 Adam Reeve](https://web.archive.org/web/20230404114230/http://adamreeve.tumblr.com/post/147120922009/pokemon-go-is-a-huge-security-risk) 决定用谷歌登录该应用时，检查该应用是否作弊。他这么做是件好事！(你也可以，[这里](https://web.archive.org/web/20230404114230/https://security.google.com/settings/u/0/security/permissions)。)

当然，Go 已经[需要一大堆权限](https://web.archive.org/web/20230404114230/https://techcrunch.com/2016/07/11/pokemon-go-wants-to-catch-almost-all-your-permissions/)——但是你可以看到它们背后的原因。它需要得到你的精确位置，访问摄像头和运动传感器，读写 SD 卡，等等。当然，当你用完了神奇球或鸡蛋时，还要向你收钱。

[![pokepermissions](img/ea439cf0516eb678fec44de32f464789.png)](https://web.archive.org/web/20230404114230/https://techcrunch.com/wp-content/uploads/2016/07/pokepermissions.png)

但是你可以完全进入你的谷歌账户？这是授予 Chrome 等平台级应用的级别。谷歌[这样描述](https://web.archive.org/web/20230404114230/https://support.google.com/accounts/answer/3466521?hl=en):

> 当您授予完全帐户访问权限时，应用程序可以查看和修改您的 Google 帐户中的几乎所有信息(但它不能更改您的密码、删除您的帐户或代表您使用 Google Wallet 进行支付)。
> 
> 这种“完全帐户访问”权限应仅授予您完全信任的应用程序，并且安装在您的个人电脑、手机或平板电脑上。

首先，为什么一个神奇宝贝游戏需要完全访问你的账户？第二，为什么没有警告用户这是他们授予的级别，并给他们一个重新考虑的机会？第三，当事情发生时，谷歌为什么不说一句话，比如“你确定你想让一个虚构的动物对抗访问你的 Gmail 和 Docs 中的机密文件的游戏吗？”(值得注意的是，Niantic 之前的 AR 游戏 Ingress 只要求部分访问。)

我们要求答案，但同时，这里有一个谜*你，读者*，可以帮助我们解决。谷歌账户的完全访问只是偶尔发生。

**(更新:**之前，这篇文章暗示谷歌账户的完全访问权限可能来自于安卓设备上的安装，但事实似乎并非如此；我们看到发生这种情况的帐户拥有来自 iOS 版本的完全访问权限，尽管它也连接了一部 Android 手机。我向 Niantic 询问了这件事和其他几件事，但还没有得到答复。这篇文章已经稍微更新，以反映这一信息。)

例如，在我安装游戏的两部手机上，运行 Android 5.2 和 6.0，它根本没有请求任何访问！(这可能是我没有收到双因素认证通知的原因)——但在一位同事的手机上，也运行 6.0，立即获得了完整的帐户访问权限。这似乎发生在一些 iPhones 上，而不是其他的。这里有规律吗？

你可以随时使用口袋妖怪训练账户注册——只是服务器太忙了，很多人没有这个选项，而是选择了谷歌。

现在，要澄清的是，我们并不是说 Niantic 或任天堂正在收集你的电子邮件或从你的 Google Drive 中吸取文件。但是首先没有理由请求这种访问，也没有办法修改它(撤销特权只会使游戏崩溃或让你退出)。也许更麻烦的是，它是在没有通知用户的情况下被请求和给出的。

在某些手机/操作系统组合上推出时，可能无法及时获得一些特定的位置或支付信息，作为权宜之计，开发人员只是要求整个帐户。

我们很快就会知道更多，但与此同时，请随意用你的手机和操作系统在下面发表评论，以及是否已被授予完全访问权限([你可以在这里查看](https://web.archive.org/web/20230404114230/https://security.google.com/settings/u/0/security/permissions))——当然，还可以吹嘘一下你收集的所有神奇宝贝。

**更新** : [《精灵宝可梦 Go》的开发者发布了一份声明，表示将解决这个权限问题](https://web.archive.org/web/20230404114230/https://techcrunch.com/2016/07/12/pokemon-go-promises-to-fix-the-bug-that-let-it-access-all-your-google-data/)，该应用没有访问用户基本账户信息以外的任何内容。