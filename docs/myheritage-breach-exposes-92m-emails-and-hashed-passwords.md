# MyHeritage 漏洞暴露 9200 万封电子邮件和散列密码

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/06/05/myheritage-breach-exposes-92m-emails-and-hashed-passwords/>

基因分析和家谱网站 MyHeritage 去年被不明身份的人入侵，他们窃取了该网站所有 9200 万注册用户的电子邮件和散列密码。没有信用卡信息，也没有(更令人不安的是)基因数据被收集。

该公司[在其博客](https://web.archive.org/web/20230306012629/https://blog.myheritage.com/2018/06/myheritage-statement-about-a-cybersecurity-incident/)上宣布了这次入侵，并解释说，一名未透露姓名的安全研究员联系了他们，警告他们他在“私人服务器”上遇到了一个文件，名为“myheritage”。里面有数百万封电子邮件和散列密码。

哈希密码是一种单向加密过程，允许敏感数据轻松存储，尽管理论上有逆转哈希的方法，但它们涉及巨大的计算能力和相当多的运气。所以密码可能是安全的，但是 MyHeritage 已经建议所有用户更改他们的密码，他们应该这样做。

这些电子邮件并没有从根本上泄露数据；多年来，像 Equifax 和雅虎这样的违规事件已经暴露了数十亿美元。它们主要与其他数据相关联。例如，黑客可以通过交叉引用这 9200 万封电子邮件的列表，将 2 和 2 放在一起，这些电子邮件的相应密码是通过其他一些漏洞知道的。这就是为什么使用密码管理器并为每个网站设置唯一的密码是件好事。

MyHeritage 确信其他数据没有被访问，这似乎是有充分理由的:

> 信用卡信息一开始并不存储在 MyHeritage 上，而是只存储在 MyHeritage 所使用的可信的第三方账单提供商(如 BlueSnap、PayPal)上。其他类型的敏感数据，如家谱和 DNA 数据，由 MyHeritage 存储在独立的系统中，与存储电子邮件地址的系统分开，它们包括额外的安全层。我们没有理由相信那些系统已经被破坏了。

当然，直到最近，该公司也没有理由相信另一个系统遭到了破坏。这是网络安全的棘手之处之一。但我们可以从这份声明中理解该公司的信用，即自入侵以来，它已密切关注其更敏感的服务器和系统，并未发现任何问题。

双因素身份验证已经在开发中，但是团队正在“加速”它的推广，所以如果你是用户，请确保在它可用时尽快设置它。

完整的报告可能需要一段时间；该公司正计划聘请一家外部安全公司来调查这一违规行为，并正在根据美国和 GDPR 等国的法律通知相关部门。

我已经要求我的遗产对一些事情进行进一步的评论和澄清，如果我得到回复，我会更新这个帖子。