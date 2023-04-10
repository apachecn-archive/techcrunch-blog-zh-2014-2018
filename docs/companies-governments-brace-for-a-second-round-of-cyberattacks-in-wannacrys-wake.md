# 在 WannaCry 之后，公司、政府准备迎接第二轮网络攻击

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/14/companies-governments-brace-for-a-second-round-of-cyberattacks-in-wannacrys-wake/>

随着世界准备在周一开始营业，[在](https://web.archive.org/web/20230307033631/http://www.reuters.com/article/us-britain-security-hospitals-idUSKBN18820S)[周五的 WannaCry 黑客攻击](https://web.archive.org/web/20230307033631/https://www.nytimes.com/interactive/2017/05/12/world/europe/wannacry-ransomware-map.html)之后，[公司和政府正准备迎接第二轮网络攻击](https://web.archive.org/web/20230307033631/http://www.reuters.com/article/us-britain-security-hospitals-idUSKBN18820S)。

事实上，安全专家已经警告说，周末出现了一个新版本的 WannaCry，它没有杀死开关协议，[在周五晚些时候阻止了最初版本的网络攻击](https://web.archive.org/web/20230307033631/https://twitter.com/charlesarthur/status/863802537601904640)。

今天早些时候，英国国家网络安全中心[发布了一个新的警告](https://web.archive.org/web/20230307033631/https://techcrunch.com/2017/05/14/uk-national-cyber-security-center-issues-new-statement-on-cyber-attack/)关于另一次攻击的可能性。

> 自上周五数十个国家的数千家私营和公共部门组织遭到全球协同勒索软件攻击以来，没有出现过持续的新的此类攻击。但是，重要的是要了解这些攻击的工作方式意味着已经发生的机器和网络损害可能尚未被检测到，并且来自恶意软件的现有感染可以在网络内传播。
> 
> **这意味着随着新的工作周的开始，在英国和其他地方，可能会出现更多的勒索案件，可能是大规模的。**

周五工作日结束时，WannaCry 黑客的初始版本被检测到，数十万台电脑受到影响。

当亚洲的工作人员周一早上醒来时，安全专家预计又一波电脑将面临勒索软件攻击。

*纽约时报*报道称，一些安全行业观察家称[第二波攻击已经开始](https://web.archive.org/web/20230307033631/https://blog.comae.io/wannacry-new-variants-detected-b8908fefea7e)。

Comae Technologies 的创始人 Matt Suiche 在他的博客上详细阐述了网络安全专家在野外发现的一些勒索软件的新变种。

> **今天(2017 年 5 月 14 日)，2 个新的**变种出现**。一个是我通过注册新域名**阻止的，另一个只是部分工作，因为它只传播和不***不*** 加密文件，由于档案损坏。
> 
> 一个新的变种被 @benkow_ 抓到并发送给我分析。我把它倒过来，找到了一个新的 kill-switch ( `*ifferfsodp9ifjaposdfjhgosurijfaewrwergwea.com*`)，我立刻**注册了它，以阻止新一波的全球攻击。然后，我与@MalwareTechBlog 和@2sec4u 同步，将新域名映射到 sinkhole 名称服务器，以馈入实时互动感染图。*这是* `*32f24601153be0885f11d62e0a8a2f0280a2034fc981d8184180c5d3b1b9e8cf*` *。***
> 
>  **一个新的变种没有被卡巴斯基捕获的杀死开关。**虽然，这个构建只*部分*起作用，因为勒索软件档案被破坏了——但是传播仍然起作用。** *这是* `*07c44729e2c570b37db695323249474831f5861d45318bf49ccf5d2f5c8ea1cd*` *。***

 **发现原始恶意软件攻击的终止开关的匿名网络安全研究人员对系统管理员提出了自己的警告。

到目前为止，您可能已经意识到最初的恶意软件攻击源自国家安全局开发的泄漏代码。该攻击利用了微软视窗系统的一个缺陷。尽管微软几个月前已经为该软件提供了补丁，但并不是每个人都更新了他们的系统，这导致了仍然匿名的黑客利用的漏洞。

根据[这位赛门铁克解释者](https://web.archive.org/web/20230307033631/https://www.symantec.com/connect/blogs/what-you-need-know-about-wannacry-ransomware)的说法，勒索软件对数据文件进行加密，并要求用户支付 300 美元的比特币赎金，如果三天后仍未付款，赎金将翻倍。一周后，加密文件将被删除。

![wcry.jpg](img/c7d320c674501222b770c170a14de38f.png)

*图 1 wanna cry 木马显示的赎金要求画面*

如果你对勒索软件攻击的工作原理感到好奇，这里有一份来自安全公司 Carbon Black 的初级读本。

受到攻击影响的公司包括西班牙电信公司、西班牙电信公司、天然气和电力供应商 Iberdrola。英国的国家健康服务医院也受到了袭击的影响。美国的联邦快递和法国的雷诺也是如此。

根据《纽约时报》的报道，德国的铁路系统、俄罗斯内政部和中国各地的大学也受到了攻击。

“毫不奇怪，全球超过 45，000 个目标受到了 WannaCry 勒索软件的攻击，”白帽渗透测试和漏洞赏金猎人初创公司 [Synack](https://web.archive.org/web/20230307033631/https://www.synack.com/) 的联合创始人兼首席技术官马克·库尔写道。“这些攻击的频率将继续呈指数级增长，因为勒索软件对犯罪企业来说是一项利润丰厚的业务。IBM 最近对 1000 名商业专业人士的调查发现，60%的受害者愿意支付赎金以安全取回数据。”

让这些攻击如此不可避免的部分原因是，几乎任何人都可以获得这些工具。潜在的黑客甚至不需要那么熟练就能部署这些恶意软件程序。

多亏了像影子经纪人[这样泄露国家安全局黑客工具](https://web.archive.org/web/20230307033631/http://money.cnn.com/2017/04/14/technology/windows-exploits-shadow-brokers/)的组织，任何有互联网连接的人都可以获得像夺取全球系统的那种恶意软件。**