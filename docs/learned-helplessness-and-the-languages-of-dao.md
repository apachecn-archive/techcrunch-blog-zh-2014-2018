# 习得性无助与道的语言

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/10/01/learned-helplessness-and-the-languages-of-dao/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

一切都很糟糕。大多数软件，甚至是关键的系统软件，都是不安全的瑞士奶酪，用胶带、气泡包装和发夹粘在一起。请看本周的黑色幽默帖子“如何在一条推特上让 Systemd 崩溃”但不仅仅是 systemd，不仅仅是 Linux，不仅仅是软件；整个行业都有错。我们错误地教导自己，别无选择。

让我们仔细看看令人捧腹的安德鲁·艾耶尔的那篇文章，因为它是一个更大问题的极好例子。“耶非决定论！”确实如此。

如果你是一个铁杆极客，你会想阅读整篇文章；如果没有，我来解释一下。Systemd 是大多数 Linux 发行版不可或缺的组件，用于引导系统等。艾耶尔找到了一个非常简单的方法来摧毁它，并继续进行哲学思考:

> 这个 bug 引发的直接问题是，什么样的质量保证过程会允许这样一个简单的 bug 存在两年多……Systemd 的问题远比这个 bug 更严重。Systemd 是有设计缺陷的。编写无 bug 软件极其困难……优秀的程序员认识到编写无 bug 软件的困难，并理解以最小化 bug 可能性或至少减少其影响的方式设计软件的重要性。systemd 开发人员对此一无所知，选择用一种不安全的内存语言编写大量不必要的复杂内容。

我认为，最后一点是最重要的一点。一切都是可怕的，因为我们使用的基本工具仍然存在缺陷，以至于在使用时不可避免地会制造出可怕的东西。这适用于从 systemd 这样的低级组件到摄像头和其他物联网设备的软件，最近[被整合成大规模 DDoS 攻击](https://web.archive.org/web/20230305141640/https://motherboard.vice.com/read/15-million-connected-cameras-ddos-botnet-brian-krebs)

——高层次的科幻抽象，如[、1.5 亿美元的以太坊道大灾难](https://web.archive.org/web/20230305141640/http://www.wsj.com/articles/investment-fund-based-on-digital-currency-to-wind-down-after-alleged-hack-1466175033)。几乎所有的软件长期以来都充满了错误和不安全，以至于我们认为这是代码的自然状态。这种习得性无助是不正确的。一切不一定都很糟糕。

原则上，代码可以通过[形式验证](https://web.archive.org/web/20230305141640/https://www.quantamagazine.org/20160920-formal-verification-creates-hacker-proof-code/)来证明其正确性。这是一件非常困难、耗时且不总是现实的事情；但是当你在谈论关键的软件，为长期而建，管理数百万机器的操作，或者数百万美元的投资，你可能至少应该考虑它。

不那么痛苦和严谨，因而更有前途的，是 [*朗赛*首创](https://web.archive.org/web/20230305141640/http://www.upstandinghackers.com/langsec):

> 语言理论方法(LANGSEC)认为互联网不安全流行是在网络栈的所有层和其他种类的软件栈中输入处理的特别编程的结果。LANGSEC 认为，获得接受不可信输入的可信软件的唯一途径是将所有有效或预期的输入视为正式语言，并将相应的输入处理例程视为该语言的识别器。

…它正通过法国安全公司 [Prevoty](https://web.archive.org/web/20230305141640/http://blog.prevoty.com/why-langsec-for-runtime-application-security-because-patterns-cant-keep-up) 等媒介稳步进入现实世界，而且不会太快。

如前所述，编程语言本身就是一个巨大的问题。大量的经验告诉我们，期望程序员用内存不安全的语言编写安全的代码是不现实的。(因此我去年发表了“[死于 C](https://web.archive.org/web/20230305141640/https://techcrunch.com/2015/05/02/and-c-plus-plus-too/) ”的帖子。)但是有希望！在悲观预言之后，安德鲁·艾耶尔继续写道:“然而，我看到了改善的迹象。对于编写传统上用 c 语言编写的系统软件来说，Go 和 Rust 是引人注目的安全语言。”

最好是好的敌人。我们不能马上从目前的不光彩状态进入一种优雅的状态。但是，作为一个行业，让我们至少设定一个*轨迹*。首先，让我们转向用更好的语言编写系统代码——这将提高安全性*和速度*。让我们转向任务关键代码的正式规范和验证。

当我们受困于遗留代码和遗留系统时，当然这仍然是大部分时间，让我们尽最大努力学习如何通过关注编程的基本规则和基础来逐步改善它。(比如 Java 和 C#程序员应该考虑去翻翻我的老同学 Ayo Agboola 的优秀的 *[练你的 Java](https://web.archive.org/web/20230305141640/http://www.pluriumpress.com/practice-your-java-level-1.html)* 和 *[练你的 C#](https://web.archive.org/web/20230305141640/http://www.pluriumpress.com/practice-your-c--level-1.html)* 的书。)不要接受“可怕”是事情的必然状态，哪怕是目前的*状态*状态。争取更好的东西。

我写这篇文章的时候，这个行业的大部分正在从传统编程转向各种风格的人工智能。我们如何正式指定一个复杂的神经网络？langsec 如何应用于我们提供给它的输入的真实世界数据？这些东西如何应用于量子计算？(如果你认为现在问这个问题还为时过早，可以看看我的朋友克里斯汀的非常酷的 [5 位量子计算机模拟器](https://web.archive.org/web/20230305141640/https://arxiv.org/abs/1606.09225)，[在 Github 上的开源](https://web.archive.org/web/20230305141640/https://github.com/corbett/QuantumComputing)。)

我，呃，实际上对最后几个问题都没有答案。但至少让我们开始问他们吧！在此期间，让我们竭尽所能，最终开始修复传统编程。这不是一个不切实际的梦想；这实际上是可能的。一旦我们接受了这一点，一切都会变得更好，我相信会的。