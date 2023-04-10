# Last.fm 入侵导致 4300 万个密码被黑

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/09/01/43-million-passwords-hacked-in-last-fm-breach/>

# Last.fm 漏洞导致 4300 万个密码被黑

关键:根据 LeakedSource 的一份报告，2012 年 3 月[发生的 Last.fm 黑客攻击中，43，570，999 个用户账户被攻破。泄密三个月后，2012 年 6 月，Last.fm](https://web.archive.org/web/20230320000850/http://www.leakedsource.com/blog/lastfm) [发布了以下声明:](https://web.archive.org/web/20230320000850/http://www.last.fm/passwordsecurity)

“我们目前正在调查一些 Last.fm 用户密码的泄露。在此之前，最近其他网站的密码泄露，以及网上发布的信息。作为预防措施，我们要求所有用户立即更改密码。”

密码的数量和黑客攻击的严重程度直到今天才被发现。密码是用无盐 MD5 散列法存储的。几乎每个存储重要用户信息的网站都使用某种形式的散列法，而不是以明文形式存储密码。哈希是一种加密数据的方法，但有些方法远远优于其他方法。

MD5 已经严重过时，部分原因是它的数学强度不足以抵抗现代的暴力破解方法。此外，Last.fm 在哈希过程中没有使用盐。Salting 是在每个个人密码的哈希中添加一个随机数字串的做法，这样可以使密码更加安全，并降低密码在网上泄露后被破解的可能性。不幸的是，Last.fm 没有采取那一步，LeakedSource 报告称，大多数密码都很容易被破解。

[本周第二次](https://web.archive.org/web/20230320000850/https://techcrunch.com/2016/08/30/dropbox-employees-password-reuse-led-to-theft-of-60m-user-credentials/)，我们的建议是，如果你在 Last.fm 上有账户，请立即更改你的密码。从 Last.fm 数据库中提取的最受欢迎的密码是 123456。说真的，现在是 2016 年——使用 LastPass 这样的平台来生成随机的复杂密码，这些密码对你注册的每个服务都是独一无二的。