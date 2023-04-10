# DreamHost 基于 OpenStack 的 EC2 竞争对手推出测试版 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/04/05/dreamhosts-openstack-powered-ec2-rival-comes-out-of-beta/>

# DreamHost 基于 OpenStack 的 EC2 竞争对手退出测试

DreamHost 最为人所知的是一项网络托管服务，但该公司也一直是面向企业的开源 OpenStack 平台的主要贡献者。在过去的几年里，它也一直在运行自己的基于 OpenStack 的云计算服务 [DreamCompute](https://web.archive.org/web/20221208140255/https://www.dreamhost.com/cloud/computing/) 测试版。

今天，DreamCompute 结束了测试，并宣布了一种新的定价模式，该模式结合了按需付费定价和可预测的月度计划。

DreamCompute 结合了 OpenStack 与 [Ceph 存储系统](https://web.archive.org/web/20221208140255/https://en.wikipedia.org/wiki/Ceph_(software))和 Dreamhost 孵化的 [Project Astara](https://web.archive.org/web/20221208140255/https://wiki.openstack.org/wiki/Astara) 网络编排服务，是亚马逊 [EC2](https://web.archive.org/web/20221208140255/https://aws.amazon.com/ec2/) 云计算服务的直接挑战者。

基于其在约 1，200 名客户中测试运行 DreamCompute 的长期经验，该团队在 DreamHost 的美国东部数据中心推出了一种全新的架构。据该公司的云副总裁 Jonathan LaCour 称，这种新的架构提供了几乎两倍于 DreamCompute 测试服务的性能。该团队大约在一年前开始研究这个新架构。正如拉库尔告诉我的那样，该团队很快意识到，例如，其用户需要 SSD 存储，他们对快速单核性能比对大量内核更感兴趣。

由于 DreamCompute 位于 OpenStack 之上，开发人员可以获得对其机器的完全 root 访问权限，并且还可以使用 OpenStack APIs 来使用它们。

DreamHost 按小时收取机器费用，但你每月支付的时间不会超过 25 天。定价从每月 4.50 美元开始。在使用传统硬盘的旧集群上，这将为您提供带有一个虚拟 CPU 的 1GB 机器，但在更快的基于 SSD 的集群上，这将只需支付 512MB 的 RAM(1GB 机器每月将花费您 6 美元)。每个 DreamCompute 群集都配有 100GB 的空闲块存储。你可以在这里找到 DreamCompute 的定价表[。](https://web.archive.org/web/20221208140255/https://help.dreamhost.com/hc/en-us/articles/217744568-What-is-DreamCompute-Predictable-Bill)

随着今天的发布，该公司还推出了一个新的知识库，以帮助其用户在其服务上运行他们的应用程序。所有信息都发布在 GitHub 上，该公司鼓励其用户分享这些信息，然后为项目做出贡献。拉库尔告诉我，随着时间的推移，该公司可能还会对贡献教程和其他文档的用户给予一些奖励(我猜，类似于 Linode 所做的事情)。