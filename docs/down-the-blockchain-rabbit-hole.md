# 侧链和闪电，新的比特币 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/06/13/down-the-blockchain-rabbit-hole/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

对于像我这样的科技专栏作家来说，比特币的伟大之处在于，它同时具有超高的电影感和技术密集度。理查德·布兰森(Richard Branson)最近在他的加勒比海私人岛屿上举办了一场“[区块链峰会](https://web.archive.org/web/20221205152551/http://www.followthecoin.com/blockchain-summit-2015-inspires-social-impact-sir-richard-branson-necker-island-blockchain-technology/)”。有一架[比特币飞机](https://web.archive.org/web/20221205152551/https://www.smallbusinessbiggame.com/contests/sbbg/entries/348)。与此同时，2015 年发布了一系列建立在比特币区块链基础上的技术上粗糙——也是技术上迷人——的提案。

如果你一直生活在法拉第笼中:区块链是一个分布式的点对点分类账系统，(通常)由加密的[工作证明](https://web.archive.org/web/20221205152551/https://en.bitcoin.it/wiki/Proof_of_work)保护，最初由一个名叫中本聪的神秘实体设计……他在 2009 年发布了世界上第一个区块链网络/协议/应用程序/货币比特币。

对大多数人来说，比特币本身已经非常深奥了(许多人仍然觉得它很可笑。)但对于加密货币爱好者来说，五分钟前，厌倦了的普通比特币已经过时了。向普通观众解释当今新的加密货币的热度是一个有趣的挑战——我拥有顶级学校的工程学位，并以编写软件为生，我仍然发现这种材料的大部分内容在初次接触时非常难以理解——但现在开始了:

**侧链元素α**

分布式比特币挖矿网络每秒执行[千万亿次运算](https://web.archive.org/web/20221205152551/https://blockchain.info/charts/hash-rate)以保持其区块链的完整性。其他区块链远没有这么安全，但他们创新更快。创业公司 [Blockstream](https://web.archive.org/web/20221205152551/http://www.blockstream.com/) 提出并开发的创新技术 *Sidechains* ，兼顾了两者的优点；新区块链的创建与比特币“挂钩”，因此价值可以在它们之间转移，可以想象比特币矿工可以通过“合并开采”自动获得这种转移

sidechains 对未来的愿景是一个由许多区块链组成的庞大的全球分散网络，一根交织的电缆而不是单一的一股，每个都有自己的协议、规则和功能——但所有这些都由比特币支持，并受到比特币采矿网络的保护，因为美元曾经由黄金支持。侧链也可以用来原型改变基本的比特币区块链。不过，有一个问题:这需要对现有的比特币协议做一点小小的调整。

在之前，我已经[写了](https://web.archive.org/web/20221205152551/https://beta.techcrunch.com/2014/04/19/bitcoin-2-0-unleash-the-sidechains/)关于这个[。然而，从本周开始，侧链不再是蒸汽制品。周一，Blockstream](https://web.archive.org/web/20221205152551/https://beta.techcrunch.com/2014/10/25/bitcoin-2-0-sidechains-and-zerocash-and-ethereum-oh-my/) [发布了第一个 alpha 版本的侧链软件](https://web.archive.org/web/20221205152551/https://www.blockstream.com/2015/06/08/714/)。

他们的“[侧链元素](https://web.archive.org/web/20221205152551/http://elementsproject.org/)”是区块链功能的集合，远远超出了比特币的区块链，包括(除其他外):

*   **保密交易**——目前，所有的比特币交易都是完全公开的，尽管是假名。[保密交易](https://web.archive.org/web/20221205152551/https://people.xiph.org/~greg/confidential_values.txt)顾名思义，向除发送者、接收者和他们指定的其他人之外的所有人隐瞒被转移的金额。最终的交易规模要大得多，但包括一个可用于存储交易或其他元数据的相当大的“memo”字段，并且仍然小于 eg [Zerocoin](https://web.archive.org/web/20221205152551/https://beta.techcrunch.com/2015/02/07/what-you-need-to-know-about-zero-knowledge/) 。(注意，这不像 Zerocash 那样保密，zero cash 通过 [zk-Snarks](https://web.archive.org/web/20221205152551/https://tahoe-lafs.org/trac/tahoe-lafs/wiki/SNARKs) 强大的近乎魔力，隐藏了参与任何交易的*参与者*。请注意，Zerocash 需要一种神秘的召唤仪式来启动它的网络。不，真的。但这是另一篇文章的主题。)
*   **隔离证人**——目前的比特币交易签名算法复杂且存在缺陷，导致了一个被称为[交易延展性](https://web.archive.org/web/20221205152551/https://en.bitcoin.it/wiki/Transaction_Malleability)的问题。隔离证人将消除这种情况，大大提高许多比特币软件的效率……并使闪电网络(见下文)等更重大的创新成为可能。
*   **新操作码** —每一笔比特币交易实际上都是用脚本语言编写的程序。这些操作码扩展了这种语言的可能性，使全新的交易形式成为可能，如彩票、向随机选择的接收者付款等。
*   **基础资产发行**——这允许 sidechain 客户发行他们自己的全新资产，就像比特币本身一样，可以在区块链安全地替代交易:代金券、优惠券、股票、债券等。我现在正式押注于第一家前沿公司是否以及何时通过“股票基础”交易上市。

Blockstream 还发布了一个“ [Alpha](https://web.archive.org/web/20221205152551/https://github.com/ElementsProject/elements/tree/alpha) ”侧链，除了最后一个功能外，所有这些功能[都已启动并运行](https://web.archive.org/web/20221205152551/https://github.com/ElementsProject/elements/blob/alpha/alpha-README.md)，与比特币测试网相耦合。(用于测试比特币软件，不会将实际价值置于风险之中。)在比特币协议没有改变的情况下，比特币和侧链之间的程序化价值转移将受到加密保护，他们正在与几家外部组织合作，以执行和验证这些转移。然而，如果协议发生变化，挂钩侧链将像比特币本身一样没有许可，也一样去中心化。

**闪电网络**

但是等等，还有呢！一个完全不同的团体发布了一份名为[闪电网络](https://web.archive.org/web/20221205152551/http://lightning.network/)的激进新提案的早期草案，该提案将在原则上把绝大多数比特币交易*移出*区块链，而不会牺牲任何可验证性或安全性。

我知道，我知道。作为一名忠实的早期科技读者，你在过去的两年里听到每个人和他们的狗赞美区块链技术的优点，比特币被认为与它有着千丝万缕的联系，现在人们突然开始谈论完全安全的区块链交易？

让我解释一下。闪电网络允许创建“微支付通道”，除了启动通道的初始交易之外，可以在不与区块链交互的情况下安全地执行多个比特币交易。不存在交易对手风险:如果任何一方停止合作，和/或没有在商定的时限内做出响应，该渠道可以关闭，其所有未结交易都将提交至区块链进行结算。

这些通道内支付将是即时的，不像目前的比特币支付，需要一个小时才能在区块链上完全验证。此外，支付可以跨多跳路径路由，就像互联网上的数据包一样——因此，你不必为每个新的交易对手创建一个通道，而是可以为少数几个联系良好的安全中介维护几个通道，并通过它们发送/接收资金。

理论上，这种分布式微支付网络——闪电网络——可以在全球范围内将比特币交易规模扩大到“每天数十亿次交易”，同时最大限度地减少区块链的使用和最低费用(直接渠道为零。)

然而，闪电网络将再次要求改变现有的比特币协议。(尽管这也是一个“软分叉”，即现有的区块链仍然完全有效。)和/或——你猜对了——闪电侧链。更重要的是，它需要的变化之一，消除事务可延展性，是由 Sidechain 元素中的隔离见证工作来处理的。(**更正** : [*所需的所有*](https://web.archive.org/web/20221205152551/https://twitter.com/adam3us/status/609810829744152576)变更都被整合到元素 Alpha 中——开箱即用。)

对两者来说都还为时尚早；但是，这些确实是有趣的时代。