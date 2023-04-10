# ProtonMail 现在支持其他客户端的 PGP 加密

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/07/26/protonmail-now-supports-pgp-encryption-with-other-clients/>

[ProtonMail](https://web.archive.org/web/20230318164232/https://protonmail.com/) 可以说是发送端到端加密邮件最简单的方式。但是加密只在默认情况下对其他 ProtonMail 用户有效。该公司正在[增加](https://web.archive.org/web/20230318164232/https://protonmail.com/blog/address-verification-pgp-support/)完全 PGP 支持，这样你就可以与使用其他应用和服务的人收发加密电子邮件。

ProtonMail 与 iMessage 或 WhatsApp 非常相似，但用于电子邮件。两个用户之间的所有通信都被无缝加密。这对最终用户是透明的，因为您不需要自己管理加密密钥。

但是加密邮件比质子邮件存在的时间更长。OpenPGP 兼容应用程序允许您在发送电子邮件之前对其进行加密和数字签名，即使您的收件人使用的不是同一个应用程序。在接收方，您可以检查发送方的签名并解密邮件。

但是 PGP 要求发送者和接收者都知道如何使用该标准。有许多扩展和插件可以在电子邮件应用程序中使用 PGP。现在，ProtonMail 让你可以直接在其服务中管理 PGP 通信。

ProtonMail 已经在后台使用 PGP 了。但是现在，这项服务正在向高级用户展示这些功能。您可以为您的联系人导入 PGP 公钥，并导出您自己的密钥与其他人共享。加密和解密是完全自动化的。

为了实现这一点，ProtonMail 正在推出一个 API，从 ProtonMail 用户那里获取公钥加密密钥。许多用户将他们的 PGP 密钥放在他们的 Twitter 个人资料或网站上。但是如果你已经知道你的收件人的 ProtonMail 邮箱地址，你可以直接从你的浏览器中获取(`https://api.protonmail.ch/pks/lookup?op=get&search=username@protonmail.com`)。

最后，公开公钥还启用了一个新功能—地址验证。如果一台服务器被入侵或者有中间人攻击，一个人可以发送一封电子邮件假装是你，但是用一套完全不同的公钥和私钥。

如果您正在处理高度敏感的信息，您现在可以手动验证特定联系人的地址。例如，如果你亲自与一个联系人会面，这个人可以向你展示他们的公钥，这样你就可以对照你的收件箱检查它。如果这两个密钥相同，您可以选择信任此密钥用于将来的通信。

这对于你的假期照片来说有点夸张，但是爱德华·斯诺登会喜欢这种功能的。ProtonMail 在给高级用户更多控制权的同时，保持了基本的加密功能。这是一个很好的入门方式，可以让你了解更多关于 PGP、公钥和私钥以及最佳实践的知识。