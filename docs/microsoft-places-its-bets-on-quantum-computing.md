# 微软押注量子计算 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/09/25/microsoft-places-its-bets-on-quantum-computing/>

在 Ignite 大会上，微软今天宣布了它的股份，并且[讨论了](https://web.archive.org/web/20221006192737/https://news.microsoft.com/features/new-microsoft-breakthroughs-general-purpose-quantum-computing-moves-closer-reality/)它在建造量子计算机方面的进展，并为开发人员提供了在现有机器上试验这种新计算模式的工具。

这里有很多问题需要解决，很少有人会声称他们了解量子计算的细节。然而，微软所做的是专注于量子计算如何工作的不同方面——这可能让它超越 IBM、谷歌和其他也在关注这一领域的竞争对手。微软所做的主要区别在于，它的系统是基于该公司之前讨论过的拓扑中的[进展。这背后的大部分理论工作来自菲尔兹奖获得者迈克尔·弗里德曼及其团队，他于 1997 年加入微软研究院。](https://web.archive.org/web/20221006192737/http://www.nature.com/news/inside-microsoft-s-quest-for-a-topological-quantum-computer-1.20774)

[![](img/03a0fc71e11065884cc295999dd33224.png)](https://web.archive.org/web/20221006192737/https://beta.techcrunch.com/wp-content/uploads/2017/09/wirebonding_qubit.jpg) “拓扑学的作用是让你拥有更好的保真度，”微软量子研究副总裁托德·霍尔姆达尔告诉我。“如果你看看我们的竞争对手，他们中的一些人拥有 3 个 9 的忠诚度，而我们可能是他们的 1000 到 10000 倍。这意味着一个逻辑量子位，我们有可能用 10 个物理量子位来实现它。”该团队本质上所做的是使用弗里德曼的理论来实现纠错，这在物理层面上对量子计算非常重要。我不会假装我真的理解什么是[拓扑量子位](https://web.archive.org/web/20221006192737/https://www.wired.com/2014/05/quantum-computing-topological-qubit/)，但它本质上比经典量子位更难被干扰(在量子计算中，即使在目前可达到的最低温度下，你也总是需要考虑一些可能干扰系统状态的噪声)。

有了 Station Q，微软现在在圣巴巴拉运营着自己的量子计算实验室，霍尔姆达尔告诉我，在过去的一年里，这个团队的规模扩大了两倍。这里的想法显然是建立一个商业量子计算机。微软是计划自己销售这款设备，还是仅仅通过 Azure 提供这款设备，还有待观察。霍尔姆达尔认为，虽然微软还没有想出商业模式，但量子计算机最自然的位置应该是在云中。毕竟，每台量子计算机都需要一台经典计算机来控制它，而且，在数据中心，你可以将量子计算机作为辅助处理单元附加到普通机器上。

[https://web.archive.org/web/20221006192737if_/https://www.youtube.com/embed/cOUrzxyng04?feature=oembed](https://web.archive.org/web/20221006192737if_/https://www.youtube.com/embed/cOUrzxyng04?feature=oembed)

视频

不过，就目前而言，这仍然是一个遥远的未来。然而，开发人员很快就能在他们自己的机器上运行微软的模拟器(尽管这些机器需要相当强大)。不过，该公司决定不仅仅发布这款模拟器。此外，该公司还开发了一种新的编程语言来编写这些量子应用程序。正如微软的 Krysta Svore 告诉我的，这里的想法是提供一个全面的全栈解决方案来控制量子计算机并为其编写应用程序。“我们喜欢谈论共同发展，”她说。“我们正在一起开发这些(硬件和软件堆栈)，以便在我们学习的过程中，您可以真正地在软件和硬件之间反馈信息，这意味着我们可以真正开发出非常优化的解决方案。”

这种编程语言采用了 C#、F#、Python 和其他语言的关键概念，但也增加了访问量子计算机功能的新功能。模拟器将允许开发人员弄清楚他们的算法是否实际可行，是否可以在量子计算机上运行，这里肯定有一个进入的障碍，例如，Svore 和 Holmdahl 都认为开始使用它应该与学习如何对 FPGA 编程没有什么不同。“如果你有一个像样的计算机科学背景，我相信三角洲比你想象的要小，”霍尔姆达尔说。

所有这些软件工具都将在今年年底上市。但是，不要期望它们是开源的。Svore 认为，无论如何，编译器的内部并不是你编写量子应用程序所真正需要的，但是你也可以这么说。微软确实开源了。NET 编译器平台。

【T2![](img/4090d1cac119d53649718b08bba46cca.png)