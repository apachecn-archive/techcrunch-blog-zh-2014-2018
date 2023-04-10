# 安全研究人员在 Equifax 阿根廷网站 TechCrunch 上发现重大缺陷

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/09/13/security-researchers-finds-gross-deficiencies-on-equifax-argentina-site/>

# 安全研究人员发现 Equifax Argentina 网站存在严重缺陷

Equifax 宣布大规模黑客攻击事件已经过去一周了，这次事件可能会泄露美国 1.43 亿消费者的财务信息，但我们仍有许多疑问。一家掌握着我们最敏感财务数据的公司怎么会允许这种事情发生？嗯，安全研究员 Brian Krebs(他在 2014 年揭露了[的目标入侵事件](https://web.archive.org/web/20221130220130/http://ajr.org/2014/06/16/reporter-mingles-criminals-cover-cybersecurity/)，[今天](https://web.archive.org/web/20221130220130/https://krebsonsecurity.com/2017/09/ayuda-help-equifax-has-my-data/)报道，该公司*在阿根廷的网站上仍然*有一些令人震惊的漏洞。

根据 [Hold Security](https://web.archive.org/web/20221130220130/https://holdsecurity.com/) 的安全研究员 Alex Holden 向 Krebs 提供的信息，该公司仍然让用户数据容易受到攻击。这家公司开始研究南美的 Equifax 网站，并且几乎立即发现，进入一个为 Equifax 阿根廷员工设计的员工门户网站来管理该国的信用纠纷非常简单。令人难以置信的是，它被用户名 *admin* 和密码 *admin* 所“保护”。显然不需要黑客天才就能进入。

一旦进入，研究人员发现大量的个人身份员工信息，包括员工姓名和电子邮件，都暴露在外。更重要的是，Krebs 报告说，管理员可以在*纯文本*中看到站点用户名，虽然他们没有直接暴露密码，但通过右键单击和查看站点源代码来暴露它们并不需要付出巨大的努力。令人难以置信的是，用户名(通常只是员工的姓氏)与密码相同。研究人员还发现，由于他们被授予了管理权限，他们可以添加、删除或修改员工记录。

从那里，研究人员能够快速访问网站上的消费者投诉记录，再次充满了 PII，包括阿根廷的社会安全号码。如果你想的话，你对 PII 可能不会更粗心了。

这里唯一要报告的好消息是，一旦 Krebs 向公司报告了这个问题，他们明智地关闭了网站，并正在调查它是如何发生的。

想到该公司可能像它之前的许多公司一样，是聪明的黑客利用社会工程进入系统内部仔细提取信息的受害者，这是一件好事，但有这样的证据表明，其中存在严重的无能，这使得这一切更加难以承受。

[![](img/7d5306b81de1eec38e58973bc8593caf.png)](https://web.archive.org/web/20221130220130/https://beta.techcrunch.com/tag/equifax-hack/)