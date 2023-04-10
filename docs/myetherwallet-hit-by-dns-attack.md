# 流行的加密钱包受到 DNS 攻击，导致一些用户的账户被清空 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/04/24/myetherwallet-hit-by-dns-attack/>

互联网上最受欢迎的钱包之一 MyEtherWallet (MEW)遭到 DNS 黑客攻击，导致一些用户丢失了他们的加密货币，此后，加密领域再次出现了担忧、眼泪和金钱损失。

[MEW 在一份声明中说](https://web.archive.org/web/20221218090431/https://www.reddit.com/r/MyEtherWallet/comments/8eloo9/official_statement_regarding_dns_spoofing_of/)“几个域名系统注册服务器在世界协调时 4 月 24 日下午 12 点左右被劫持，将用户重定向到一个钓鱼网站。”并非所有在劫持期间访问该网站的人都受到影响，但 MEW 表示，其中“大多数”人一直在使用谷歌的 DNS。

“我们目前正在核实哪些服务器被锁定，以帮助尽快解决这一问题，”该公司补充说，并确认此后已保护其网站。该公司建议那些曾经使用谷歌 DNS 的人改用 [Cloudflare 的](https://web.archive.org/web/20221218090431/https://blog.cloudflare.com/announcing-1111/)。

维基百科、[微软、谷歌和贝宝的国别版本](https://web.archive.org/web/20221218090431/https://arstechnica.com/information-technology/2012/11/google-microsoft-paypal-other-romanian-sites-hijacked-by-dns-hackers/)和[甚至银行](https://web.archive.org/web/20221218090431/https://www.wired.com/2017/04/hackers-hijacked-banks-entire-online-operation/)以前也曾遭受过类似的攻击。

像这样的事件不会直接危及网站，但是，在 MEW 的案例中，它导致一些用户访问不安全的网站。从那里，那些输入私钥信息而没有意识到自己被网络钓鱼的人面临着数据被另一端的攻击者窃取的风险。有了这些信息，攻击者就可以访问他们的帐户并清空其中的内容。(注意:这是建议人们永远不要手动输入私钥的一个非常好的原因，也是强烈建议使用安全硬件的原因。)

很难量化像这样的攻击的影响，因为 MEW 是一个如此受欢迎和受信任的服务，而 MEW 表示，它仍在收集关于到底发生了什么的信息。

据 Coindesk 报道，150，000 美元或 216 乙醚被盗，但数字可能更高。[一名诈骗追踪者](https://web.archive.org/web/20221218090431/https://disqus.com/by/409H/)发现了攻击中使用的两个钱包([在这里](https://web.archive.org/web/20221218090431/https://etherscan.io/address/0xf203a3b241decafd4bdebbb557070db337d0ad27)和[在这里](https://web.archive.org/web/20221218090431/https://etherscan.io/address/0x1d50588c0aa11959a5c28831ce3dc5f1d3120d29))，它们导致了一个看起来像是钱包的东西([在这里](https://web.archive.org/web/20221218090431/https://etherscan.io/address/0x39683abdba389bad9d39fadb82a45bc56244133f))今天收集了超过 520 个乙醚。按今天每 ETH 700 美元的价格计算，大约需要 365，000 美元。

实际金额可能更高。持有钱包导致[一个更大的钱包](https://web.archive.org/web/20221218090431/https://etherscan.io/address/0xb3aaaae47070264f3595c5032ee94b620a583a39)，它在以太网中有超过 1700 万美元的余额和源源不断的交易。这并不是说 1700 万美元被盗——这不太可能——但攻击者可能使用其他尚未被跟踪的钱包，但最终会找到这个更大的钱包。

除了使用 Trezor 或 Ledger 等硬件，crypto wallet 用户——嗯，一般的互联网用户——在处理私人信息时，应该检查网站的 SSL(显示在浏览器栏中域名的左侧)是否安全。

这是水电部给社区的信息。

“用户，在进行任何交易之前，请确保有一个绿色栏 SSL 证书，上面写着“MyEtherWallet Inc”。我们建议用户运行 MEW (MyEtherWallet)的本地(离线)副本。我们敦促用户使用硬件钱包来存储他们的加密货币，”它在 Reddit 的一份声明中说。

那些寻找水电部替代品的人可以求助于 MyCrypto，这是由水电部的一位前联合创始人于 2 月份创立的，提供类似的服务。两个网站都不保存用户的密码或信息；相反，它们允许检查账户，并使交易能够被发送到区块链，之后它们被运送到预定的接收者。

*披露:作者拥有少量加密货币。足以获得一种理解，不足以改变一种生活。*