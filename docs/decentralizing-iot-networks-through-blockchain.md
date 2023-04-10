# 通过区块链分散物联网网络 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/06/28/decentralizing-iot-networks-through-blockchain/>

本·迪克森是一名软件工程师，也是

[TechTalks](https://web.archive.org/web/20221004033327/https://bdtechtalks.com/)

.

More posts by this contributor

想象一下这样一台洗衣机，它可以自动联系供应商并在洗涤剂不足时下订单，执行自助服务和维护，从外部资源下载新的洗涤程序，安排其周期以利用电价，并与对等设备协商以优化其环境；一辆联网的汽车，足够智能，可以找到并选择零件和服务的最佳交易；一个制造工厂，机器知道什么时候需要修理它的一些零件，而不需要人工干预。

所有这些场景——以及更多——都将因物联网(IoT)而成为现实。许多历史上不太适合计算机的[行业已经被连接到互联网的数十亿物联网设备所改变；随着 T2 数十亿人加入竞争，其他行业也将效仿。](https://web.archive.org/web/20221004033327/http://uk.businessinsider.com/internet-of-things-in-manufacturing-2016-2?r=US&IR=T)

[可能性几乎是数不清的](https://web.archive.org/web/20221004033327/https://bdtechtalks.com/2016/05/10/iot-and-machine-learning-are-invading-our-lives-is-it-a-good-thing/)，尤其是当物联网的力量与机器学习等其他技术的力量相结合时。但是，随着数十亿智能设备想要在它们之间以及与它们的主人进行交互，一些主要的障碍将会浮出水面。虽然当前支持物联网通信的模型无法应对这些挑战，但科技公司和研究人员希望通过区块链来应对这些挑战，这项技术构成了著名的比特币的主干。

## 集中式模型的问题是

当前的物联网生态系统依赖于集中式代理通信模型，也称为服务器/客户端范式。所有设备都通过拥有巨大处理和存储能力的云服务器进行识别、认证和连接。设备之间的连接将只能通过互联网，即使它们恰好相距几英尺。

虽然这种模式已经连接了几十年的通用计算设备，并将继续支持我们今天看到的小规模物联网网络，但它将无法响应未来巨大物联网生态系统日益增长的需求。

[现有物联网解决方案价格昂贵](https://web.archive.org/web/20221004033327/http://venturebeat.com/2014/08/24/the-internet-of-things-will-cost-companies-more-than-theyre-ready-for/)因为与集中式云、大型服务器群和网络设备相关的基础设施和维护成本很高。当物联网设备增长到数百亿时，必须处理的通信量将大幅增加这些成本。

即使前所未有的经济和工程挑战被克服，云服务器仍将是一个瓶颈和故障点，可能会扰乱整个网络。这一点尤其重要，因为更加关键的任务，如[人类健康和生命将依赖物联网](https://web.archive.org/web/20221004033327/https://bdtechtalks.com/2016/05/24/can-we-trust-iot-in-healthcare/)。

> 没有连接所有设备的单一平台。

此外，设备及其支持的云基础设施之间所有权的多样性使得机器对机器(M2M)通信变得困难。没有连接所有设备的单一平台，也不能保证不同制造商提供的云服务能够互操作和兼容。

## 分散物联网网络

物联网联网的分散方法可以解决上述许多问题。采用标准化的点对点通信模式来处理设备之间的数千亿次交易，将显著降低安装和维护大型集中式数据中心的相关成本，并将在构成物联网网络的数十亿台设备之间分配计算和存储需求。这将防止网络中任何单个节点的故障导致整个网络停止崩溃。

然而，建立对等通信会带来一系列挑战，其中最主要的是安全问题。众所周知，[物联网安全不仅仅是保护敏感数据。](https://web.archive.org/web/20221004033327/https://beta.techcrunch.com/2015/10/24/why-iot-security-is-so-critical/)提议的解决方案必须维护巨大物联网网络中的隐私和安全，并为交易提供某种形式的验证和共识，以防止欺骗和盗窃。

## 区块链方法

[区块链](https://web.archive.org/web/20221004033327/http://blogs.wsj.com/cio/2016/02/02/cio-explainer-what-is-blockchain/)为点对点通信平台问题提供了一个优雅的解决方案。它是一种允许创建交易的分布式数字分类帐的技术，该分类帐在网络的节点之间共享，而不是存储在中央服务器上。参与者在区块链注册，以便能够记录交易。该技术使用加密技术来验证和识别参与节点，并允许它们安全地将交易添加到分类帐中。参与网络的其他节点对交易进行验证和确认，从而消除了对中央机构的需求。

该分类帐是防篡改的，不能被恶意行为者操纵，因为它不存在于任何单个位置，并且中间人攻击不能上演，因为没有单个通信线程可以被拦截。区块链使无信任的点对点消息传递成为可能，并且已经通过比特币等加密货币在金融服务领域[证明了自己的价值，提供有保障的点对点支付服务，而不需要第三方经纪人。](https://web.archive.org/web/20221004033327/http://searchcio.techtarget.com/feature/Blockchain-technology-to-disrupt-financial-legal-fields)

科技公司现在正在考虑将区块链的可用性移植到物联网领域。

> 区块链在物联网中的应用并非没有缺陷和不足。

这个概念可以直接移植到物联网网络来处理规模问题，允许数十亿设备共享同一个网络，而不需要额外的资源。区块链还通过提供一个每个人都拥有平等股份和利益的标准，解决了不同供应商之间的权力冲突问题。

这有助于打开 M2M 通信，这在以前的模式下几乎是不可能的，并允许实现全新的用例。

## 区块链在物联网中的具体应用

物联网和区块链的结合已经获得了势头，并得到了初创公司和科技巨头的认可。IBM 和三星推出了他们的概念验证系统 [ADEPT](https://web.archive.org/web/20221004033327/http://www.zdnet.com/article/is-blockchain-the-key-to-the-internet-of-things-ibm-and-samsung-think-it-might-just-be/) ，该系统使用区块链来支持下一代物联网生态系统，每天将产生数千亿次交易。

在第一批描述物联网中使用区块链的论文之一中，IBM 的 Paul Brody 描述了新设备如何在制造商组装时首先在通用区块链中注册，然后在出售给经销商或客户后转移到区域区块链，在那里它们可以与共享区块链的其他设备自动交互。

物联网和区块链的结合也创造了[循环经济](https://web.archive.org/web/20221004033327/https://beta.techcrunch.com/2016/04/02/intelligent-assets-as-an-enabler-of-the-transition-to-a-circular-economy/)的可能性，并液化了资产的容量，资源可以共享和重复使用，而不是购买一次，使用后丢弃。由区块链平台领导者[以太坊](https://web.archive.org/web/20221004033327/https://www.ethereum.org/)主办的物联网黑客马拉松对区块链驱动的物联网概念进行了测试，其中[展示了一些有趣的想法](https://web.archive.org/web/20221004033327/http://www.rs-online.com/designspark/electronics/eng/blog/enabling-new-smart-device-applications-the-iot-blockchain-hackathon-in-london)，包括能源共享和电力及燃气计费领域。

[Filament](https://web.archive.org/web/20221004033327/http://filament.com/) 是另一家投资物联网和区块链的初创公司，专注于农业、制造业和石油天然气等工业应用。Filament 使用被称为 Taps 的无线传感器来创建低功耗自主[网状网络](https://web.archive.org/web/20221004033327/http://internetofthingsagenda.techtarget.com/feature/Using-mesh-networking-to-interconnect-IoT-devices)，用于数据收集和资产监控，而不需要云或中央网络机构。该公司使用区块链技术来识别和认证设备，并通过比特币对网络和数据服务收费。

[物联网链](https://web.archive.org/web/20221004033327/http://www.chainofthings.com/)是一个正在探索区块链在处理物联网规模和安全问题中的作用的联盟。在最近于伦敦举行的黑客马拉松中，该组织在一个案例研究中展示了[区块链和物联网的使用](https://web.archive.org/web/20221004033327/https://thestack.com/iot/2016/06/02/can-blockchain-save-iot-from-itself/)，该案例研究涉及一个太阳能堆栈，旨在提供可靠和可验证的可再生数据，加快激励结算并减少欺诈机会。该系统简化了太阳能电池板连接到数据记录器的过程，跟踪产生的太阳能量，安全地将数据传输到节点，并将其记录在分布式账本上，该账本在更广泛的全球节点网络中同步。

## 警告和挑战

区块链在物联网中的应用并非没有缺陷和不足，还有一些障碍需要克服。[首先，比特币开发者](https://web.archive.org/web/20221004033327/http://www.nytimes.com/2016/01/17/business/dealbook/the-bitcoin-believer-who-gave-up.html?_r=0)对底层区块链技术的架构存在争议，其根源在于网络增长和交易数量增加带来的问题。其中一些问题将不可避免地适用于区块链到物联网的扩展。这些挑战[已经被科技公司](https://web.archive.org/web/20221004033327/http://www.coindesk.com/ibm-reveals-proof-concept-blockchain-powered-internet-things/)认识到，包括侧链、树链和迷你区块链在内的几种解决方案正在测试中，以解决这个问题。

处理能力和能耗也是一个关注点。区块链交易的加密和验证是计算密集型操作，需要相当大的马力来执行，这是许多物联网设备所缺乏的。存储也是如此，因为分类帐的大小开始增长，需要冗余地存储在网络节点中。

此外，正如[玛奇纳研究](https://web.archive.org/web/20221004033327/https://machinaresearch.com/)分析师 [Jeremy Green 解释](https://web.archive.org/web/20221004033327/http://internetofthingsagenda.techtarget.com/blog/IoT-Agenda/Will-blockchain-make-the-leap-from-cryptocurrency-to-smart-machines)的那样，由区块链支持的自主物联网网络将对制造商正在寻求的商业模式构成挑战，这包括具有持续收入流的长期订阅关系，并且将需要商业和经济模式的重大转变。

现在说区块链是否是快速发展的物联网产业问题的明确答案还为时过早。它还不完美；尽管如此，对于物联网的未来来说，这是一个非常有前景的组合，其中分散的、自治的网络将起到决定性的作用。