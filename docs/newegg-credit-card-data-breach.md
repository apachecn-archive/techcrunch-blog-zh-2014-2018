# 黑客在新蛋数据泄露事件中窃取了客户的信用卡

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/19/newegg-credit-card-data-breach/>

# 新蛋数据泄露事件中黑客窃取了顾客的信用卡

在长达一个月的数据泄露后，新蛋公司正在清理其网站。

RiskIQ 的威胁研究员 Yonathan Klijnsma 告诉 TechCrunch，黑客在这家在线零售商的支付页面上注入了 15 行刷卡代码，并在 8 月 14 日至 9 月 18 日期间保持了一个多月。这种代码将不知情的顾客的信用卡数据转移到一台由黑客控制的服务器上，该服务器有一个相似的域名——很可能是为了避免被发现。服务器甚至使用了一个 HTTPS 证书来融入其中。

该代码也适用于桌面和移动用户——尽管尚不清楚移动用户是否会受到影响。

这家在线电子产品零售商在事件响应公司 Volexity 联系它后，于周二删除了代码，该公司首先发现了刷卡恶意软件，并[报告了其发现](https://web.archive.org/web/20230331000351/https://www.volexity.com/blog/2018/09/19/magecart-strikes-again-newegg)。

新蛋是美国最大的零售商之一，2016 年收入 26.5 亿美元。该公司宣称每月有超过 4500 万的独立访客，但不清楚有多少客户在此期间完成了交易。

在给客户的一封电子邮件中，新蛋首席执行官李修贤表示，该公司“尚未确定哪些客户账户可能受到了影响。”当联系到新蛋公司的发言人时，他没有立即发表评论。

Klijnsma 称这一事件是“另一次精心伪装的攻击”，看起来与最近英国航空公司信用卡被盗的[和更早的](https://web.archive.org/web/20230331000351/https://techcrunch.com/2018/09/06/british-airways-customer-data-stolen-in-data-breach/)[ticket master 信用卡被盗的](https://web.archive.org/web/20230331000351/https://techcrunch.com/2018/06/28/bank-says-ticketmaster-knew-of-breach-months-before-taking-action/)几乎一模一样。像那次入侵一样，RiskIQ 将新蛋信用卡盗窃案归咎于 Magecart 集团，这是一个黑客团体，对易受攻击的网站进行有针对性的攻击。

根据研究，两次略读攻击中使用的代码几乎相同。

“新蛋的漏洞显示了 Magecart 运营商的真实范围，”Klijnsma 说这些攻击并不局限于某些地理位置或特定行业，任何处理在线支付的组织都是目标。"

像以前的盗卡活动一样，他说黑客“整合了受害者的支付系统，与基础设施融为一体，并尽可能长时间地呆在那里。”

在此期间输入信用卡数据的任何人都应该立即联系他们的银行。