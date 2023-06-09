# 约翰·迈克菲的“无法破解”的 Bitfi 钱包再次遭到黑客攻击

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/08/30/john-mcafees-unhackable-bitfi-wallet-got-hacked-again/>

如果安全社区只能告诉你一件事，那就是“没有什么是不可攻击的”除了约翰·迈克菲的加密货币钱包，它只能被破解，直到它不被破解——两次。

安全研究人员现在开发了第二种攻击，他们说可以从未经修改的 Bitfi 钱包中获取所有存储的资金。Android 驱动的 120 美元钱包依靠用户生成的秘密短语和“盐”值(如电话号码)对秘密短语进行加密加扰。这个想法是，这两个独特的价值确保您的资金保持安全。

但是研究人员表示，可以提取秘密短语和盐，从而生成私钥并窃取资金。

使用这种“冷启动攻击”，即使 Bitfi 钱包关闭，也有可能窃取资金。下面有个视频。

研究人员[萨利姆·拉希德](https://web.archive.org/web/20230402011039/https://twitter.com/spudowiar)和[瑞安·卡斯特卢奇](https://web.archive.org/web/20230402011039/https://twitter.com/ryancdotorg)作为几名自称“THCMKACGASSCO”(以他们的首字母命名)的安全研究人员团队的一部分，发现并构建了这些漏洞。两位研究人员在 TechCrunch 发布之前分享了他们的成果。在视频中，拉希德设置了一个秘密短语和盐，并运行本地漏洞从设备中提取密钥。

拉希德告诉 TechCrunch，这些密钥在内存中的存储时间比 Bitfi 声称的要长，这使得他们可以在不擦除内存的情况下在硬件上运行代码。从那里，攻击者可以提取内存并找到密钥。拉希德说，这个漏洞运行不到两分钟。

“这种攻击既可靠又实用，不需要专门的硬件，”Pen Test Partners 的安全研究员 Andrew Tierney 证实了这种攻击。

蒂尔尼是第一次 Bitfi 攻击背后的黑客之一。迈克菲支持的公司悬赏 250，000 美元，奖励任何能够实施其制造者认为的“成功攻击”的人但是 Bitfi 拒绝支付，辩称黑客攻击不在奖金范围内，而是求助于在 Twitter 上发布威胁。

蒂尔尼说，这种新的攻击“在精神上符合赏金的要求，即使它不符合 Bitfi 设定的具体条款。”

迈克菲本月早些时候说，“当有人得到硬币时，钱包就被黑了。”

Bitfi 运营副总裁比尔·鲍威尔(Bill Powel)在一封电子邮件中告诉 TechCrunch，该公司将黑客定义为“任何允许攻击者访问钱包中资金的行为。”

他说:“因为这个设备不存储私钥，所以才引发了不可破解的声明。”

当记者追问时，Powel 并没有说明冷启动攻击的具体说法。在给 Bitfi 的邮件中被复制的 McAfee 没有回应。

在研究人员发布视频的一个小时内，Bitfi 在[的一份推特声明](https://web.archive.org/web/20230402011039/https://twitter.com/Bitfi6/status/1035279307617259523)中表示，它已经“聘请了一位经验丰富的安全经理，他正在确认研究人员已经发现的漏洞。”

“立即生效，我们正在关闭目前的奖金计划，这已经引起了研究人员可以理解的愤怒和沮丧，”它补充说。

该声明还表示，它将不再在其网站上使用“不可破解”的说法。

Rashid 说，他没有立即发布漏洞代码的计划，以防止估计数千名 Bitfi 用户面临风险。

就在上个月， [Bitfi 获得了 Pwnie Award](https://web.archive.org/web/20230402011039/https://www.pentestpartners.com/security-blog/bitfi-research-receives-pwnie-award-for-lamest-vendor-response/) 最差供应商响应奖，这是在黑帽大会上颁发的传统奖项，奖励在安全问题上反应最差的公司。