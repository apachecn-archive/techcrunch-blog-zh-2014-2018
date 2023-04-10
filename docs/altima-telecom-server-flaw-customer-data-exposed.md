# 网站漏洞暴露了加拿大 ISP 的整个客户数据库 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/10/01/altima-telecom-server-flaw-customer-data-exposed/>

# 网站漏洞暴露了加拿大 ISP 的整个客户数据库

加拿大互联网提供商 Altima Telecom 修复了其网站中的一个缺陷，该缺陷可能会使攻击者能够完全访问其客户数据库。

客户数据库连接到该公司的网站，但可以远程访问一个盲目的 SQL 注入攻击。落水狗安全公司(Underdog Security)的创始人戴利·博尔达(Daley Borda)发现了这个漏洞，并将其报告给了 TechCrunch，我们又将此报告给了 Altima。

Altima Telecom 自称是加拿大最大的独立互联网服务提供商之一，为蒙特利尔和多伦多提供服务。

根据 Borda 的说法，该数据库包含 427 个表，包含数百万条客户记录，包括账单数据、支持票和其他用户数据。虽然研究人员可以通过在浏览器的地址栏中输入命令来探测数据库，但他说恶意攻击者可以轻松地转储其内容并下载整个数据库。

他还发现了几个存储信用卡数据的数据库列，包括卡号、有效期、安全码和地址。

当联系到 Altima 时，Altima 的首席执行官 Frank Yang 告诉 TechCrunch，该数据库使用加密密钥管理服务进行保护。但是当我们向几个安全研究人员询问这个漏洞时，他们说一个成功的注入攻击会表现为来自合法用户的请求。

“我们真的很感谢你和安全研究员让我们注意到这一点，”杨说。“我们非常严肃地对待这件事。”

这是一个令人惊讶的简单缺陷，可能会造成重大损失，即使对于一个中等规模的 ISP。Altima 的曝光是互联网提供商一系列安全事件中的最新一起。康卡斯特已经[修补了几个漏洞](https://web.archive.org/web/20230206100549/https://techcrunch.com/2018/05/21/comcast-is-leaking-the-names-and-passwords-of-customers-wireless-routers/)，这些漏洞[允许不当访问](https://web.archive.org/web/20230206100549/https://www.buzzfeednews.com/article/nicolenguyen/a-comcast-security-flaw-exposed-millions-of-customers)客户数据。纽约有线电视提供商 RCN 最近承认以明文形式存储客户密码。