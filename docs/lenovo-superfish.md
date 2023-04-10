# 联想电脑附带广告软件，构成严重的安全威胁 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/02/18/lenovo-superfish/>

# 联想电脑附带广告软件，构成严重的安全威胁

联想今天陷入了困境，因为一个重大的安全漏洞被发现，可能会影响其整个消费 PC 系列。

Superfish 是一个广告软件程序，它随联想的所有消费电脑一起提供，使用中间人证书将广告注入互联网浏览器。如果遭到破坏，该服务可能会授权第三方访问用户的浏览器数据。

我们联系了联想请其置评，但在撰写本文时尚未收到该公司的回复。

在一月份的一个客户论坛上，[公司代表 Mark Hopkins 证实了](https://web.archive.org/web/20221007233327/https://forums.lenovo.com/t5/Lenovo-P-Y-and-Z-series/Lenovo-Pre-instaling-adware-spam-Superfish-powerd-by/m-p/1863174/highlight/true#M79882)客户的怀疑，即联想预装了来自[的“视觉搜索”公司的软件。他进一步解释说，由于“一些问题”，该软件已被“暂时删除”，这显然包括无法解释的弹出窗口。他补充说，Superfish 已被告知向市场上现有的设备推送更新。](https://web.archive.org/web/20221007233327/http://thenextweb.com/insider/2015/02/19/lenovo-caught-installing-adware-new-computers/)

预装不受消费者欢迎，可以理解的是，消费者希望他们的设备开箱后是干净的，但实际上，一些硬件公司确实为了经济利益而安排这种安排。除了超级鱼在浏览器中弹出的不便和安装它的需要，该软件似乎构成了严重的安全威胁，因为[它使用自签名根](https://web.archive.org/web/20221007233327/https://forums.lenovo.com/t5/Security-Malware/Potentially-Unwanted-Program-Superfish-VisualDiscovery/m-p/1860408/highlight/true#M1697)，这可以允许它从用户的网络浏览器中收集数据。

此外，正如黑客新闻所指出的，第三方可能会生成超级鱼证书的密钥，并利用它来进行邪恶的活动。

像银行这样的个人数据领域将是一个明显的关注领域，根据这条推文，一个伪造的 bankofamerica.com 证书——只是关于这个主题的许多[中的一个——显示了什么是可能的:](https://web.archive.org/web/20221007233327/https://twitter.com/search?q=%23superfish&src=typd)

https://Twitter . com/kenn white/status/568270748638318593/photo/1

更糟糕的是，似乎删除 Superfish 软件并没有消除联想机器上的证书(和威胁)。

霍普金斯对超级鱼如何整合工作和不工作做出了声明:

> Superfish 技术纯粹基于上下文/图像而非行为。它既不剖析也不监控用户行为。它不记录用户信息。它不知道用户是谁。用户既不会被跟踪，也不会成为目标。每个会话都是独立的。

然而，用户数据和安全受到威胁的事实，理所当然地引起了联想客户和安全专家的警觉。

与此相关的是，据报道，英国间谍机构已经禁止在他们的组织中使用联想设备，因为这些设备存在漏洞，可能会被黑客攻击。