# 为超融合基础设施重构网络

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/03/14/reimagining-the-network-for-a-hyper-converged-infrastructure/>

基图·科卢里撰稿人

[Kittu Kolluri](https://web.archive.org/web/20230301141841/https://www.linkedin.com/in/kittukolluri/)

是的创始人和董事总经理

[Neotribe Ventures](https://web.archive.org/web/20230301141841/https://www.neotribe.vc/)

，专注于对发展突破性技术的早期至成长期公司的战略投资。

More posts by this contributor

**编者按:** *基图·科卢里是 NEA 的普通合伙人，专注于 IT 和能源技术投资。他的投资包括 Box、Aerohive Networks、Braintree、BloomReach、VeloCloud 和 Cohere Technologies 等。*

你的力量取决于你最薄弱的环节，这是当今互联网最大的问题。二十多年来，互联网的支柱——网络——一直生活在阴影中，被快速增长的互联网经济和一群有很大损失的强大在位者的重压所压制。

自 SaaS 早期以来，科技界已经为创新设定了惊人的速度。如果云打破了一切(事实也的确如此)，那么如果没有弹性，我们就一无是处——在交付“一切即服务”、大数据和移动性的竞赛中，我们要扫除每一个障碍。我们已经进化成了沉迷于设备、吞噬应用的带宽饕餮者——同时哄骗和哄骗底层架构来管理远超其设计承受能力的负载。

这种自上而下的创新的影响通常是从广域网(WAN)的角度来说明的，但是如果不断蔓延的 WAN 是一股上涨的浪潮，那么数据中心正在争先恐后地抵御洪水。

我们没有视而不见；事实上，恰恰相反。但是从技术的角度来看，这个架构不能简单地修复，它必须被重新设计。在一个由行业巨头、遗留系统和组织内部动态组成的复杂生态系统中，这是一个不小的壮举。然而有一点一直很清楚:这个问题只能通过推动技术进步来解决。

我们做到了，尽管是在孤岛中推进:计算、存储和网络。在云计算出现之前，应用程序将资源分成三个整齐的组。这种做法一直很有效，但后来失败了:虚拟化带来了计算层的横向扩展。

现在，存储必须向计算靠拢，以确保性能和可扩展性。融合存储解决了邻近性问题，正如像 [Nutanix](https://web.archive.org/web/20230301141841/http://www.nutanix.com/) 、 [SimpliVity](https://web.archive.org/web/20230301141841/http://www.simplivity.com/) 和 [Springpath](https://web.archive.org/web/20230301141841/http://www.springpathinc.com/) 这样的公司所展示的那样，但由此带来的东西向流量的增加将瓶颈转移到了网络上。

以基于主机的虚拟化为形式的软件定义网络(SDN)(由 Nicira/ [VMWare](https://web.archive.org/web/20230301141841/http://www.vmware.com/) 和 [PLUMgrid](https://web.archive.org/web/20230301141841/http://www.plumgrid.com/) 等公司首创)将控制平面与数据平面分离开来，但并未解决底层物理网络基础设施问题。

在当今移动第一、应用丰富且始终在线的世界中，我们的基础架构方法必须更加全面，这意味着向基于云的架构的转变。这一直是 NEA 企业投资组合中的一个主导主题，但在过去的一两年里，我们看到了转型的加速。

随着一些非常有趣的创业游戏和一些现任者的大动作，虚拟覆盖已经迅速成为这个新生市场中受欢迎的方法。尽管受制于思科设备，思科的以应用为中心的基础设施( [ACI](https://web.archive.org/web/20230301141841/http://www.cisco.com/c/en/us/solutions/data-center-virtualization/application-centric-infrastructure/index.html) )堆栈技术在概念上类似于虚拟网络覆盖。有趣的是，思科现在计划在其交换机上支持开源协议，以使不购买其 ACI 堆栈的客户更容易实现虚拟覆盖。

在创新网络操作系统虚拟化的初创公司中， [Pluribus Networks](https://web.archive.org/web/20230301141841/http://www.pluribusnetworks.com/) 脱颖而出有几个原因。其软件定义的结构允许组织聚合计算、网络、存储和虚拟化。

在早期的解决方案将网络置于传输层的情况下，Pluribus 围绕网络更具战略性和智能性的角色构建了自己的价值主张。有大量的行业活动验证了 Pluribus 的开放软件定义的结构方法；特别值得注意的是[脸书楔](https://web.archive.org/web/20230301141841/http://www.theregister.co.uk/2014/06/18/facebook_open_switch/)。

凭借硬件和软件部署方案，该公司迄今已从一个包括硅谷内部人士和全球战略投资者的投资集团筹集了近 1 亿美元。其他初创公司也开始追求类似的模式——阿尔卡特朗讯分拆出来的 [Nuage](https://web.archive.org/web/20230301141841/http://www.nuagenetworks.net/) 最初在服务提供商领域起步，专注于网络功能虚拟化，但现在越来越专注于企业数据中心的 SDN。同样，[大交换机网络](https://web.archive.org/web/20230301141841/http://www.bigswitch.com/)从基于主机的网络虚拟化转变为基于结构的模型。

考虑到数据中心之外的问题，许多初创公司都在解决企业与其分支机构之间不断扩大的差距——有些公司采用 SDN 解决方案(即 Nuage 的虚拟化网络服务)，另一些公司则直接专注于 WAN 环境的虚拟化。

[Velocloud](https://web.archive.org/web/20230301141841/http://www.velocloud.com/) 就是其中之一，他们构建了云路由器来解决点对点 WAN 优化无法解决的问题，并通过公共互联网连接实现了业务级性能。

具有讽刺意味的是，随着应用领域的拆分和功能的分离，底层基础设施正在转变为软件定义的单层网状结构，即由计算、网络和存储组成的超融合基础设施。但考虑到应用程序激增、大数据、内容流和在线协作推动的流量和消费的爆炸式增长，底层架构变得越来越灵活和动态是合理的。

这种转变由来已久，但事实证明，解决方案比任何人预期的都更简单、更优雅。在我看来，互联网平淡无奇的外表可能是云计算转型中最大的机遇。

*信息披露:NEA 是 Pluribus、Springpath 和 Velocloud 的投资者。*