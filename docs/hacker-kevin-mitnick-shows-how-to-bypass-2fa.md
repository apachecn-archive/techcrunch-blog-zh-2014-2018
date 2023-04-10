# 黑客凯文·米特尼克展示如何绕过 2FA 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/05/10/hacker-kevin-mitnick-shows-how-to-bypass-2fa/>

# 黑客凯文·米特尼克展示如何绕过 2FA

一个新的漏洞允许黑客通过将用户发送到一个虚假的登录页面，然后窃取用户名、密码和会话 cookie 来欺骗双因素身份验证请求。

KnowBe4 首席黑客官凯文·米特尼克在一段公开视频中展示了这次黑客攻击。通过说服受害者访问类似“LunkedIn.com”的域名，并获取登录、密码和身份验证代码，黑客可以将凭据传递到实际站点并获取会话 cookie。一旦做到这一点，黑客可以无限期登录。这实际上是使用一次性 2FA 代码来欺骗登录和获取数据。

“凯文的一个白帽黑客朋友开发了一个工具，利用社会工程策略绕过双重认证——它可以被武器化用于任何网站，”KnowBe4 首席执行官斯图·斯朱尔曼说。“双因素身份认证旨在提供额外的安全层，但在这种情况下，我们清楚地看到，您不能单靠它来保护您的组织。”

白帽黑客库巴·格雷茨基创建了这个名为 [evilginx](https://web.archive.org/web/20230121134117/https://breakdev.org/evilginx-advanced-phishing-with-two-factor-authentication-bypass/) 的系统，并在他的网站上一篇极其详尽的[帖子中描述了它的实现。](https://web.archive.org/web/20230121134117/https://breakdev.org/evilginx-advanced-phishing-with-two-factor-authentication-bypass/)

Sjouwerman 指出，反网络钓鱼教育非常重要，如果受害者了解安全性以及点击进入你邮箱的链接的危险，像这样的黑客攻击是不可能完成的。为了证明这一点，Sjouwerman 给我发了一封邮件，看起来是马特·伯恩斯·(matt@techcrunch.com 写给我的，内容是关于一篇文章中的一个打字错误。当我点击它时，我被转移到一个 SendGrid 重定向网站，并被转储到 TechCrunch——但有效载荷可能会更邪恶。

![](img/7234db1e72f9f749cea1f74d0237204d.png)

![](img/fc8fd8f45a1b93654cd05267799e5fef.png)

“这凸显了新学校安全意识培训和模拟网络钓鱼的必要性，因为人们确实是你的最后一道防线，”Sjouwerman 说。他估计黑客将在未来几周内开始尝试这种技术，并敦促用户和 IT 经理强化他们的安全协议。

【YouTube = https://www . YouTube . com/watch？v=xaOX8DS-Cto]