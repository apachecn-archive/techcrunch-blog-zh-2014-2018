# 加密货币的不安全性:IOTA、BCash 和更多 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/08/09/cryptocurrency-insecurity-iota-bcash-and-too-many-more/>

加密货币:由才华横溢的工程师构建的迷人技术的怪异集合体；一种全新的、潜在重要的经济学形式；…还有炒作——机器张狂——胡说八道。因此，正如你所料，它们还结合了最先进的弹性工程和滑稽的小丑车所谓的安全性。是的，没错——我想说的是 IOTA，以及(在一定程度上)比特币现金。

现代安全实践包括:理解并承诺[负责任的披露](https://web.archive.org/web/20221203140329/https://en.wikipedia.org/wiki/Responsible_disclosure)；让第三方安全研究人员能够访问您；提供臭虫奖励； [fuzzing](https://web.archive.org/web/20221203140329/https://en.wikipedia.org/wiki/Fuzzing) 你的代码；等等。它们还包括一些有价值的老生常谈，比如“[不要推出自己的密码](https://web.archive.org/web/20221203140329/https://motherboard.vice.com/en_us/article/wnx8nq/why-you-dont-roll-your-own-crypto)”这里的 *crypto* 是指 *cryptography* ，意思是，永远永远使用经过实践检验的加密算法和实现。不要试图从零开始构建自己的。你会后悔的。

IOTA，[目前](https://web.archive.org/web/20221203140329/https://coinmarketcap.com/)是世界上第十大最有价值的加密货币，它对这句格言采取了…坚定的反对立场。他们不仅推出了自己的密码，他们还推出了自己的基本单元，认为二进制不够好，三进制比比特和字节好得多。

我承认，我的一部分对这种古怪行为艺术的超现实主义怀有勉强的敬意。唉，这种半钦佩并没有延伸到最近的传奇故事，其中 a)他们推出了自己的密码；b)麻省理工和波士顿大学的研究人员在其中发现了一个缺陷；c) IOTA 首先说这个缺陷是故意的，然后，很明显，它是由一个不完美的 AI (!);一场[壮观的口水战](https://web.archive.org/web/20221203140329/https://motherboard.vice.com/en_us/article/ywq44k/a-5-billion-cryptocurrency-iota-has-enraged-cryptographers-leaked-emails)(在那些党派和其他几个党派之间)爆发了。然后，昨天，[麻省理工学院数字货币项目的负责人 Neha Narula](https://web.archive.org/web/20221203140329/https://www.media.mit.edu/people/narula/overview/) ，在黑帽的一次演讲中展示了去年的工作——尽管这项工作源于去年 […](https://web.archive.org/web/20221203140329/https://twitter.com/matthew_d_green/status/1027197543271358465)

今天早上我采访了 Narula，她仍然很惊讶地说，在她看来，似乎 IOTA 认为她昨天的讲话将揭示一个新的、以前未披露的弱点。他们对软件安全如何工作以及负责任的披露意味着什么的根本误解令人震惊。

你可能会认为 IOTA 是一个极其荒谬的项目，以至于用它作为例子是不公平的。但如果是这样，请记住加密货币仍然是一个非常怪异的领域，许多投入大量资金的人无法区分荒谬的项目和严肃的项目。几天前，我参观了拉斯维加斯的“加密货币夜总会”，这个名字叫 MORE 再合适不过了；总的想法是，人们既可以投资 MoreCoin(是的，真的),又可以用它在拉斯维加斯和类似的目的地进行更好的访问/聚会。无论你认为这是一个有效的概念还是一个疯狂的快速致富计划，这都是加密货币越来越多地针对不成熟公众的一个例子。对于它的目标受众来说，更多的货币和比特币没有太大的区别；任何技术上的荒谬都不是成功的障碍。

但如果你想谈些更严肃、更高调的话题，没问题；让我们来谈谈 Narula 的[最新帖子](https://web.archive.org/web/20221203140329/https://medium.com/@neha/reducing-the-risk-of-catastrophic-cryptocurrency-bugs-dcdd493c7569)，这篇帖子描述并关注比特币现金中的一个漏洞，比特币是比特币基地交易的极少数货币之一。几个月前，开发人员科里·菲尔兹(Cory Fields)发现，产生比特币现金的硬分叉包括对比特币共识代码的一些重构……因此可以制作一个恶意块，将比特币现金分成两个独立的区块链。

这将非常糟糕，几乎肯定会大幅降低比特币现金的价值，并可能被用于双重消费攻击；这意味着，鉴于比特币现金的价值和流动性，这是一个可以被用来产生数百万美元现金的漏洞。幸运的是，菲尔兹是一个令人钦佩的人，他决定做正确的事情。

但是…怎么做？联系谁？他认为，拥有比特币现金回购承诺权的人；但是它们都没有提供安全的公众联系方式。这是可以用来诈骗数百万美元的信息，它不能以明文形式通过电子邮件发送——更重要的是，如果其他人发现了这个漏洞，但这个核心开发人员是已知唯一发现它的人，他将成为一个巨大的目标。当没有出口可以披露的时候，你怎么能进行负责任的披露呢？

最后，菲尔兹找到了一种方法。([一种很复杂的方式](https://web.archive.org/web/20221203140329/https://medium.com/@coryfields/http-coryfields-com-cash-48a99b85aad4))。)并且 bug 已经修复。但他遇到的困难凸显了一个事实，随着加密货币的成熟，其安全政策和程序也需要随之成熟。向那些已经在这条道路上走得很好的人致敬，比如[以太坊](https://web.archive.org/web/20221203140329/https://bounty.ethereum.org/)、 [EOS](https://web.archive.org/web/20221203140329/https://hackerone.com/eosio) 和[Tezos](https://web.archive.org/web/20221203140329/https://tezos.com/bugbounty/)；和/或那些以武器化的无知回应的人。