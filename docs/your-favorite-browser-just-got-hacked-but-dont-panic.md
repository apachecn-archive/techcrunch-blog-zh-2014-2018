# 你最喜欢的浏览器刚刚遭到黑客攻击，但不要惊慌

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/03/20/your-favorite-browser-just-got-hacked-but-dont-panic/>

![browsers](img/aec6ea3ca8dfa7239ec5dd30dcfdbc93.png)

怎么才能知道你“最喜欢的浏览器”是什么？没关系，真的；如果它是四种最流行的浏览器中的任何一种——Chrome、Internet Explorer、Firefox 或 Safari——它刚刚被成功利用。

过去的一周标志着第八届年度 [Pwn2Own](https://web.archive.org/web/20230320150828/https://cansecwest.com/) ，来自四面八方的安全研究人员在这里展示他们的才华。目标？展示流行浏览器的最新版本，获得大量现金回报。

好消息是:由于竞争的性质，在浏览器背后的公司有机会修补之前，这些攻击的细节都不会公开。因此，虽然这里被利用的漏洞可能潜伏在你的浏览器中，但在它们被清理之前，你*可能*没有被它们发现的危险。

例如，Mozilla 告诉我，他们将在今天结束前给 Firefox 打补丁。在这篇文章发表时，没有其他浏览器制造商对我们的置评请求做出回应。

Pwn2Own 中的[对“利用”](https://web.archive.org/web/20230320150828/http://zerodayinitiative.com/Pwn2Own2015Rules.html)的定义相当直接:“修改程序或进程的标准执行路径，以便允许执行任意指令”。

换句话说:突破浏览器的安全系统，让它运行不应该运行的代码。除了“浏览恶意内容所需的操作”之外，不允许任何用户交互。

每个研究人员有 30 分钟的时间在他们从未接触过的机器上演示他们的利用，每台机器都运行完全补丁版本的操作系统。需要澄清的是:这些 bug 中的大部分是几天/几周研究的结果——它们不是研究人员在他们 30 分钟的演示窗口中发现的。

**以下是各浏览器的表现:**

*   在 Internet Explorer 中演示了 4 个错误(在 Windows 8.1 上测试)
*   在 Mozilla Firefox 中演示了 3 个错误(在 Windows 8.1 上测试)
*   Safari 中演示了 2 个 bug(在 OS X Yosemite 上测试)
*   在 Chrome 中演示了 1 个 bug(在 Windows 8.1 上测试)

(*注:在任何人说“哈！还好我经营歌剧！”，记住 Opera 从 2013 年 5 月就开始基于 Chrome/Chromium 了。所以 Chrome 的漏洞可能也会影响 Opera。*)

与此同时，研究人员还演示了 Adobe Reader、Flash 和 Windows 本身的漏洞。

最后一个浏览器漏洞，也就是 Chrome 中发现的那个，实际上导致了比赛历史上最大的一笔奖金:惊人的 11 万美元。Chrome 已经是所有浏览器中支付金额最高的了，因为它是出了名的难以利用——但是研究员 JungHoon Lee 因为它的风格获得了一些奖金。他为最初的 bug 得到了 75000 美元，为让他的代码在系统级运行得到了 25000 美元，另外 10000 美元是因为 bug *也*在 Chrome 的测试版中工作。

JungHoon 也是 Safari 中发现的一个漏洞(5 万美元)和 IE11 中的一个漏洞(6.5 万美元)背后的研究人员，他当天总共净赚了 22.5 万美元。不错的发薪日。

在为期两天的比赛结束时，总共向参赛者支付了 557，500 美元。