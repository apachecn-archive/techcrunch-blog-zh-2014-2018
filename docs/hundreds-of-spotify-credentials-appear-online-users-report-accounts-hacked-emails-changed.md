# 数百份 Spotify 凭证出现在网上——用户报告账户被黑，电子邮件被更改 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/04/25/hundreds-of-spotify-credentials-appear-online-users-report-accounts-hacked-emails-changed/>

一份包含数百个 Spotify 账户凭证的列表——包括电子邮件、用户名、密码、账户类型和其他细节——出现在网站 Pastebin 上，这似乎是一个可能的安全漏洞。在通过电子邮件对受害者进行随机抽样调查后，我们确认这些用户的 Spotify 账户仅在几天前被侵入。然而，Spotify 表示，它“没有遭到黑客攻击”，其“用户记录是安全的”。

鉴于这些账户信息是 Spotify 特有的，而不是 Spotify 上的一组通用凭证，因此不清楚这些账户信息是从哪里获得的。

除了电子邮件和登录信息之外，Pastebin 帖子还详细说明了帐户的类型(例如，家庭、高级)、订阅自动续订的时间以及帐户创建的国家。帐户列表不仅限于美国，还包括世界各地的许多用户。

![spotify-pastebin](img/0ba421bb244057013e127d4edb36eb59.png)

Spotify 过去曾处理过 T2 的安全事件，所以人们不能马上认为像这样的邮件列表与新的数据泄露有关。有可能是一份之前被泄露的账户名单仍在流传。我们尝试的账户中只有一个允许登录，这也让我们对这一特殊事件的新近性产生了怀疑。

但我们联系的受害者告诉我们的却不是这样。

到目前为止，已经有超过六个人做出了回应，证实他们最近确实遇到了 Spotify 账户被盗的问题。他们通过多种方式意识到了这个漏洞——例如，一个人说他发现他保存的歌曲列表中添加了他没有添加的歌曲。

另一个人也发现他的账户被一个不知名的第三方使用。

“我怀疑我的账户上周被黑客入侵了，因为我看到了我从未听过的‘最近播放’的歌曲，所以我修改了密码，注销了所有设备，”这位不愿透露姓名的受害者告诉我们。

![spotify-overview](img/be1810363af16ab6d26613db617a5ac1.png)

其他几个人说他们被踢出了 Spotify——其中一个甚至在流媒体音乐播放中。

当试图重新登录时，这些用户发现他们的帐户电子邮件已被更改为不属于他们的新电子邮件地址。

为了解决这个问题，用户表示他们必须与 Spotify 客服合作，恢复他们的账户访问权限。

到目前为止，在报告的案例中，Spotify 没有在违规后立即联系受害者，Spotify 也没有代表他们主动重置他们的密码。

这似乎与 Spotify 发言人今天在被问及这一可能的违规行为时向我们提供的声明相矛盾:

> “Spotify 没有被黑客攻击，我们的用户记录是安全的。我们定期监控 Pastebin 和其他网站。当我们找到 Spotify 凭据时，我们会首先验证它们是否可信，如果可信，我们会立即通知受影响的用户更改他们的密码。

但有可能 Spotify 仍在验证帐户凭据，这需要时间。

据我们目前接触的许多用户说，这个问题发生在上周。然而，帕斯捷潘的日期是 4 月 23 日。(TechCrunch 拒绝链接到 Pastebin 页面以保护受害者。)

![spotify-email-reset](img/544c0bdd3f47a2efe9b66146e2b25fda.png)

一些受害者现在才开始处理后果。一对夫妇说，他们收到了电子邮件通知，称他们的密码已于周日重置。

一名受害者告诉我们，“……我肯定是被黑客攻击了，然后昨晚试图在谷歌上搜索 Spotify 黑客新闻’但没有结果。”。“我昨晚在手机上打开 Spotify 时注意到了这一点，看到有人在别的地方使用我的账户。”

未知方重置了他们的电子邮件地址，删除了一个播放列表，将音乐保存到他们的设备中，并开始关注一个新的播放列表。

其他人仍在试图向 Spotify 证明他们是合法的账户所有者。

另一位用户告诉我们:“…这个人可以在没有第二次验证的情况下更改我的电子邮件地址，现在我要想方设法关闭我的账户。”。

“我必须先联系 Spotify，现在还在进行中，”第三个人说。“他们没帮上什么忙，到目前为止，我只是成功地锁定了我的账户。”

由于 Spotify 在重置用户密码方面的延迟，许多受害者告诉我们，他们遇到的问题不仅限于流媒体服务。

不幸的是，由于人们经常在其他网站上重复使用他们的密码，一些人报告说他们的其他账户也被黑客入侵，包括他们的脸书、优步、Skype 甚至他们的银行账户。

目前还不清楚为什么对这一事件负责的未知第三方会想要实际上*使用*Spotify 用户登录来播放音乐——特别是当这提醒用户违规时。通常情况下，黑客会简单地收集凭证，然后再出售，这使得这个特殊的事件很奇怪。

*随着信息的公开，还会有更多。*

**更新**:我们了解到，Spotify 的问题可能是由于该服务缺乏双重认证。最有可能的情况是，Spotify 的用户从其他网站重新使用了他们的密码，而他们就是在那里第一次被盗的。(这就是为什么 Spotify 可以说它的服务器没有被入侵。)

一个可能执行这种黑客攻击的程序是 Sentry MBA，它可以强制网站在设定的时间间隔登录账户。黑客为各种网站配置这种配置，然后在论坛上与他人分享这些“配置”，这些人随后攻击帐户并发布数据转储以获得声誉。

也就是说，虽然 Spotify 可能没有被直接攻破，但它缺乏双重身份认证，这使得其用户的账户容易受到这种攻击。