# 研究人员发现允许免费乘坐优步的漏洞

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/03/04/researcher-finds-bug-that-allows-free-uber-rides/>

# 研究人员发现允许免费乘坐优步的漏洞

优步修补了其代码中的一个漏洞，允许研究人员——以及任何可能发现该问题的人——在不付费的情况下招呼优步乘坐。

安全研究员阿南德·普拉卡什(Anand Prakash)在 8 月份发现了这个漏洞，并获得了优步的许可，可以在美国和印度进行测试。他成功地利用了这个漏洞，在两个地方都免费乘车。

普拉卡什通过优步的[漏洞奖励计划](https://web.archive.org/web/20230206214929/https://hackerone.com/uber)报告了这个问题，该计划奖励发现和报告安全漏洞的黑客现金。许多科技公司运营 bug bounty 项目，作为加强产品安全性的一种方式。根据漏洞的严重程度以及是否影响其他用户，黑客在优步可以赚 100-10000 美元。优步在普拉卡什报告漏洞的当天就修复了漏洞，并付给他 5000 美元，但普拉卡什一直等到本周才公开讨论这个漏洞。

“攻击者可能滥用这一点，从他们的优步账户中获取无限免费乘车，”他在[的博客帖子](https://web.archive.org/web/20230206214929/http://www.anandpraka.sh/2017/03/how-anyone-could-have-used-uber-to-ride.html)中解释说。

错误发生在指定支付方式时。普拉卡什在一个概念验证视频中展示了他可以指定一种无效的支付方式，用简单的字符串表示，如“abc”或“xyz”，并且不会为旅程付费。

“优步的漏洞奖励计划与世界各地的安全研究人员合作修复漏洞，即使这些漏洞不会直接影响我们的用户。我们感谢阿南德的持续贡献，并很高兴奖励他一份出色的报告，”优步的发言人说。

普拉卡什在优步的漏洞赏金计划中排名第 14，并经常向其他公司提交漏洞报告，如[脸书](https://web.archive.org/web/20230206214929/http://www.csmonitor.com/World/Passcode/Security-culture/2016/1003/Hackers-for-good-How-Anand-Prakash-rescued-Facebook)，在那里他也是排名第一的黑客。