# 不，新的 Gmail API 不会扼杀 IMAP 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/06/26/no-the-new-gmail-api-is-not-killing-imap/>

昨天，在谷歌的 I/O 开发者大会上，该公司宣布了一种新的方式，通过其全新的 Gmail API，开发者可以构建与 Gmail 集成的应用程序。该 API 旨在允许对消息、线程、标签和草稿进行编程访问，最初被一些人误解为谷歌试图“杀死 IMAP”，这是一种提供电子邮件访问、检索和存储的旧电子邮件协议。

这种困惑似乎很大程度上是因为一篇流量很高的[华尔街日报文章](https://web.archive.org/web/20221208171909/http://online.wsj.com/articles/google-opens-gmail-making-it-more-of-a-platform-for-developers-1403719202)中的措辞，该文章最初称，新的 API 将*取代 IMAP，IMAP 是应用程序与大多数电子邮件服务进行通信的一种常见但复杂的方式。*(这篇文章已经用新的语言更新，说“代替”而不是“替换”)

谷歌的开发者文档[也支持这一点:新的 Gmail API 不会扼杀 IMAP——至少现在不会——但它会让 Gmail 应用程序开发更容易。](https://web.archive.org/web/20221208171909/https://developers.google.com/gmail/api/)

谷歌在一篇详细介绍该 API 新特性的博客文章中解释说，[Gmail API 并不提供所有操作的完整收件箱访问；正如开发者文档](https://web.archive.org/web/20221208171909/http://googleappsdeveloper.blogspot.ca/2014/06/introducing-new-gmail-api.html)[所述](https://web.archive.org/web/20221208171909/https://developers.google.com/gmail/api/)，它是对不需要“完全电子邮件客户端访问”的应用程序进行细粒度控制。

相反，对于需要浏览你的收件箱、寻找电子收据、行程或订单确认的应用程序来说，这种 API 会工作得很好；允许您安排稍后发送电子邮件的选项；CRM 应用程序；电子邮件“暂停”按钮；还有更多。在这些不需要访问完整收件箱的情况下，Gmail API 会比使用 IMAP 更快地执行搜索或查找特定的电子邮件主题。

虽然 Gmail API 意味着谷歌正在邀请开发者开发更多挖掘你最隐私的社交网络(即你的电子邮件收件箱)的应用程序，但它也在以一种实际上更好地尊重这些数据的敏感性的方式这样做。

现在，如果用户想要授权一个只执行一种功能的应用程序，比如代表用户发送邮件，但不检索收到的邮件，Gmail API 可以允许这一点，而在此之前，用 IMAP 构建的同一应用程序将意味着开发者必须访问你的所有电子邮件，才能让他们的应用程序工作。

然而，Gmail API 没有启用移动电子邮件客户端的阵容，例如[伴奏](https://web.archive.org/web/20221208171909/https://beta.techcrunch.com/2014/02/20/acompli-raises-7-3m-series-a-from-redpoint-others-to-fix-mobile-email/)、[云魔术](https://web.archive.org/web/20221208171909/https://cloudmagic.com/)、[拳击手](https://web.archive.org/web/20221208171909/http://www.getboxer.com/)或[兴致](https://web.archive.org/web/20221208171909/https://beta.techcrunch.com/2014/04/18/gusto-debuts-a-smarter-more-powerful-email-app-for-iphone/)。这些应用程序仍然需要使用 IMAP 和 SMTP 等旧协议，至少在谷歌决定进一步扩展 Gmail API 以包含 IMAP 的所有功能之前，如果该公司选择走这条路的话。

Gmail API 现在处于测试阶段，谷歌在大范围发布前征求开发者的反馈。

[YouTube https://www.youtube.com/watch?v=UhdiQmS3kDs]