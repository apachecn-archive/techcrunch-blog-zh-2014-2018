# 谷歌开源其跷跷板负载平衡器 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/01/29/google-open-sources-its-seesaw-load-balancer/>

# 谷歌开源了它的跷跷板负载平衡器

Google [今天宣布](https://web.archive.org/web/20221205160254/http://google-opensource.blogspot.com/2016/01/seesaw-scalable-and-robust-load.html)它是开源的跷跷板——一个基于 Linux 的负载平衡系统。这个项目的代码是用谷歌的 Go 语言编写的，现在可以在 [Apache 许可](https://web.archive.org/web/20221205160254/https://github.com/google/seesaw/blob/master/LICENSE)下在[的 GitHub](https://web.archive.org/web/20221205160254/https://github.com/google/seesaw) 上获得。

谷歌网站可靠性工程师 Joel Sing 在今天的公告中写道，谷歌在 2012 年曾使用两种不同的负载平衡系统。然而，两者都“提出了不同的管理和稳定性挑战。”因此，为了解决这个问题，他和他的团队开始寻找新的解决方案，因为当时可用的解决方案不能满足谷歌的需求，他们开始编写自己的解决方案。

Sing 写道:“这些要求并不复杂——我们需要能够处理单播和任播[VIP](https://web.archive.org/web/20221205160254/https://en.wikipedia.org/wiki/Virtual_IP_address)的流量，利用 [NAT](https://web.archive.org/web/20221205160254/http://www.linuxvirtualserver.org/VS-NAT.html) 和 [DSR(也称为 DR)](https://web.archive.org/web/20221205160254/http://www.linuxvirtualserver.org/VS-DRouting.html) 执行负载平衡，并对后端执行充分的健康检查。”。“最重要的是，我们需要一个易于管理的平台，包括配置更改的自动部署。”

因为其中一个平台已经使用了 [Linux 虚拟服务器](https://web.archive.org/web/20221205160254/http://www.linuxvirtualserver.org/whatis.html) (LVS)进行网络级负载平衡，所以团队坚持使用这个平台。除此之外，Google 还实现了一个模块化的多进程架构和一些故障转移和恢复服务。

“经过一段时间的集中开发工作，我们完成并成功部署了 Seesaw v2，作为现有两个平台的替代品，”Sing 写道。“总的来说，它让我们提高了服务可用性，降低了管理开销。”

值得注意的是，虽然这个项目出自谷歌，但开源版本并不是谷歌的官方产品。所以不要指望公司会提供任何官方支持。