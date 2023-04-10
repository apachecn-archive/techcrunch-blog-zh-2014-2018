# 微软希望通过其新的 Coco 框架 TechCrunch 使区块链网络为企业做好准备

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/08/10/microsoft-wants-to-make-blockchain-networks-enterprise-ready-with-its-new-coco-framework/>

人们对区块链的兴趣空前高涨，但仍有大量技术问题需要解决，特别是对于那些希望将这项技术用于智能合同和其他用例的企业。对他们来说，吞吐量、延迟、治理和保密性等问题仍然是使用区块链的主要绊脚石。凭借其新的 [Coco 框架](https://web.archive.org/web/20230125152716/http://www.aka.ms/cocoframework)，微软希望解决这些问题，并使区块链更适合企业。

在本周早些时候的一次采访中，微软 Azure 的首席技术官(和[偶尔的小说家](https://web.archive.org/web/20230125152716/http://www.trojanhorsethebook.com/))马克·鲁西诺维奇告诉我，公司发现用户对区块链技术很感兴趣。他们喜欢分布式账本的总体想法，但每秒只能处理少量交易的系统不适合他们——他们想要的是每秒可以处理一千或更多交易的技术。

Coco 框架通过引入可信执行环境(TEE)解决了区块链的这些基本问题。这里的基本思想是，你有一个可信的盒子，你可以信任把你的区块链代码。这种信任是通过英特尔的软件卫士扩展或 Windows 的虚拟安全模式等工具建立的，因为它是一个开放的框架，所以它也可以支持其他可用的 tee。有了这些 t 恤，你就可以建立一个可信的飞地网络，所有这些飞地都同意它们正在运行的分类账和 Coco 代码(这是一个英特尔和其他公司也在过去[试验过的概念](https://web.archive.org/web/20230125152716/https://www.coindesk.com/intel-hardware-security-blockchains/))。

一旦你有了这些可信的飞地，所有其他的部分就都到位了。因为您可以信任对分类帐的更新，所以您不需要执行任何工作证明，这大大提高了事务处理速度。在典型的分类帐中，这需要几秒钟甚至几分钟。但有了 enclaves，这就不是问题了，微软表示，在其原型设置中，Coco 和以太坊每秒可以处理多达 1600 次交易。得益于此，区块链网络——当与类似于 [Paxos](https://web.archive.org/web/20230125152716/https://en.wikipedia.org/wiki/Paxos_(computer_science)) 的协议相结合以确保一致性时——变成了一个可用的数据库。

企业还希望确保他们的一个供应商看不到您向另一个供应商下的订单。当你的账目公开时，这是一个很难解决的问题。然而，Coco 在类似以太坊(或任何其他分类帐，因为该框架是分类帐不可知的)的分类帐之上添加了一个保密层。实现这一点只需要对微软原型中的以太坊协议做一些小的改动。

Coco 支持的另一个特性是治理。为了解释这一点，Russinovich 举了一个想使用区块链网络的银行财团的例子。谁可以在这个网络中增加另一家银行？Coco 治理系统允许联盟的成员为像这样的决策制定投票规则。

这里重要的是，Coco 框架将与任何分类帐协议兼容，并且几乎可以在任何地方运行——云中或内部，以及支持兼容的可信环境的任何操作系统和虚拟机管理程序上。R3 Corda ，英特尔孵化的 [Hyperledger 锯齿](https://web.archive.org/web/20230125152716/https://intelledger.github.io/introduction.html)和 [J.P. Morgan Quorum](https://web.archive.org/web/20230125152716/https://github.com/jpmorganchase/quorum) 将与 Coco 整合他们的分布式分类账。

英特尔软件和服务集团副总裁兼平台安全部门总经理 Rick Echevarria 在今天的发布会上表示:“我们很高兴能与微软合作，将区块链引入企业。“我们共同的客户对区块链的潜力感到兴奋。英特尔致力于通过提高基于我们技术的解决方案的可扩展性、隐私性和安全性，在英特尔硬件上加速实现 Azure 支持的区块链的价值。”

不过，先别太兴奋。微软将在 2018 年初为 Coco 开源代码。Russinovich 告诉我，团队仍在强化代码，并为开源做准备。不过，该公司今天正在制作技术白皮书和演示。