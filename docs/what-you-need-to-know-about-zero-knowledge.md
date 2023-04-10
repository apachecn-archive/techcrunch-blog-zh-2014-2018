# 你需要了解的零知识

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/02/07/what-you-need-to-know-about-zero-knowledge/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

匿名？隐私？多么古怪。我们生活在一个被越来越多的 T2 相机、越来越多的传感器、越来越多的无人机、越来越多的数据、越来越少的可以隐藏的东西装饰的世界。 [TLS](https://web.archive.org/web/20230318113352/http://en.wikipedia.org/wiki/Transport_Layer_Security) 和 [Tor](https://web.archive.org/web/20230318113352/http://www.torproject.org/) 可以隐藏你的在线浏览，没错——但是，实际上，你做的任何重要的事情，无论在线还是离线，都可以很容易地被审计和跟踪。

没错，你仍然可以发送私人信息。来自[Open whispers systems](https://web.archive.org/web/20230318113352/https://whispersystems.org/)的 Signal/RedPhone/TextSecure 是安全消息传递的黄金标准，[暗物质](https://web.archive.org/web/20230318113352/http://arstechnica.com/security/2014/10/the-secure-smartphone-that-wont-get-you-beaten-with-rubber-hoses/)看起来很有趣。但是如果你想超越信息传递进入交易，你的运气就用完了。

以比特币为例。它作为黑市的首选货币而声名狼藉——但它也是“在某种意义上，有史以来最不匿名的货币，因为任何拥有比特币账户的人都可以观察到每一笔交易，”引用经济学家大卫·弗里德曼的话。问问所谓的丝绸之路首脑罗斯·乌布里希特就知道了，他的笔记本电脑里有 70 万比特币，可直接追踪到丝绸之路的账户。

你不能用没有标记的比特币要求支付；没有这回事。声称“大型欧洲公司可能会将比特币视为一种保护其数据的选择，并使其对美国保密”目前是滑稽可笑的。当然，你可以“翻滚”你的比特币支付，即将它们与陌生人的支付混合在一起，或者或许使用像[黑暗钱包](https://web.archive.org/web/20230318113352/http://www.wired.com/2014/07/inside-dark-wallet/)这样的服务(本质上是一种分布式翻滚器)——但你必须绝对信任该服务以保护你的匿名性……而不是保留你的钱。

这是单一全球分布式账本不可避免的缺点，对吧？谁都可以看。合情合理。

…或者你会这么想。

但是你低估了今天的数学家和密码学家，后果自负。我给你 [Zerocoin](https://web.archive.org/web/20230318113352/http://en.wikipedia.org/wiki/Zerocoin) ，一种执行真正匿名加密货币交易的方式。它旨在作为比特币的扩展，但也完全可以作为一种独立的“零币”加密货币。

这怎么可能？这个概念非常简单:零硬币是从一个集体托管池中抽取的，这个托管池是在主币的区块链上定义、标注和维护的，当零硬币从托管池中出现时，它的交易历史就会被清除。交易通过*零知识证明*来验证:一种证明真理的数学方法，无需透露任何进一步的验证信息。(要了解更多细节，请参见 Zerocoin 的创始人之一马修·格林的这本精美的[插图初级读本](https://web.archive.org/web/20230318113352/http://blog.cryptographyengineering.com/2014/11/zero-knowledge-proofs-illustrated-primer.html)，或者 Zerocoin 的原始论文[。)](https://web.archive.org/web/20230318113352/http://spar.isi.jhu.edu/~mgreen/ZerocoinOakland.pdf)

这不仅仅是一个迷人的概念；一家名为 [Moneta](https://web.archive.org/web/20230318113352/https://moneta.cash/about.html) 的初创公司已经倒闭，而[实施了](https://web.archive.org/web/20230318113352/https://moneta.cash/technology.html)zero coin 协议(以及区块链的其他改进。)他们的“创世纪板块”——他们的区块链——计划在接下来的几个月发射。

与此同时，Zerocoin 的人们已经将他们最初的提议扩展成一个更加匿名的协议，叫做 Zerocash。Zerocash 并非完全不可信；它必须是由可信实体最初建立的[。然而，此后，其区块链将允许不包含任何关于其发送方*或*接收方*或*金额的公开信息的交易——但所有这些事情仍然可以使用零知识证明来验证。(确实，“](https://web.archive.org/web/20230318113352/http://zerocash-project.org/q_and_a)[这样的证明不到 300 字节长，只需要几毫秒就可以验证](https://web.archive.org/web/20230318113352/http://zerocash-project.org/how_zerocash_works)。)令人难忘的是，它们被称为 zk-SNARKs，意为“零知识简洁的非交互式知识论证”。)

…但我们不要太兴奋。让我们给这些狂热的梦想泼一点冷水吧。有数百个潜在的比特币继承者，但每一个都没能取代比特币之王。比特币的技术似乎越来越过时了(仅仅五年！)但它的网络效应似乎让它无懈可击。尽管去年有如此多的嘘声和哀叹，一枚比特币仍然价值超过 200 美元。这是超乎寻常的。像维基百科一样，比特币在理论上可能行不通，但在实践中几乎不可阻挡；任何时候都不会有其他加密货币将它从宝座上拉下来。

这就是为什么*挂钩侧链*如此重要。我已经在之前[写过关于他们的](https://web.archive.org/web/20230318113352/https://techcrunch.com/2014/10/25/bitcoin-2-0-sidechains-and-zerocash-and-ethereum-oh-my/)；基本上，它们是一种跨越许多区块链交织的方式来交换比特币，从而扩展协议，而不必以某种方式推翻比特币的主导地位。(sidechains 背后的初创公司[block stream 最近融资 2100 万美元，其创始人中有几名核心比特币开发者。)](https://web.archive.org/web/20230318113352/http://insidebitcoins.com/news/gregory-maxwell-demo-sidechains-to-be-available-in-a-few-months/29531)

在我看来，Zerocoin 和 Zerocash 是侧链的低挂果实。只需将你的比特币转移到一个实现其中一种协议的侧链上，瞧，比特币立即匿名；你可以发送或接收金钱，同时保持数学上完美的隐私。这是否会产生实际和监管方面的影响？你打赌。会一直是好事吗？实际上，可能不会。但是在一个逐渐成为万物的全景监狱的世界里，一次一个带摄像头的遥控设备，任何保护隐私的东西都是好东西。为零知识欢呼三声。

尽管这只是第一步。我将把最后的话留给莫内塔的联合创始人[李永迎](https://web.archive.org/web/20230318113352/https://moneta.cash/about.html):

> Moneta 项目的愿景是帮助显著推进比特币技术作为侧链。作为一个侧链，我们希望帮助人们认识到，有可能让比特币变得快如闪电，更加隐私，更具可扩展性。例如，人们往往认为比特币仅限于每秒 7 次交易，永远无法与 Visa 竞争。通过对协议的一些修改，我们可以将这个数字增加 100 倍。此外，随着可伸缩性的提高，交易费用也会降低。想想所有新的市场和行为，如果我们可以将比特币的交易费用从美分的数量级降低到百分之一美分的数量级……我们希望传达的是，比特币的底层协议实际上可以得到显著的改进——不仅仅是微小的改进，而是 10 倍或 100 倍的改进。