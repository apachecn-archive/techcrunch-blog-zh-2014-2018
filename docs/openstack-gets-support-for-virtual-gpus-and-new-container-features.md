# OpenStack 获得对虚拟 GPU 和新容器功能的支持 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/28/openstack-gets-support-for-virtual-gpus-and-new-container-features/>

[OpenStack](https://web.archive.org/web/20221207212857/https://www.openstack.org/) 是一个开源基础设施项目，旨在为企业提供相当于私有云的 AWS，今天宣布推出其第 17 版，被称为“Queens”在所有这些版本之后，您可能会认为 OpenStack 社区没有多少新东西可以添加到项目中，但正如大型公共云不断添加新服务一样，OpenStack 也是如此。

[![](img/c15b91ea12d130ab0418df26417cc3e9.png)](https://web.archive.org/web/20221207212857/https://tctechcrunch2011.files.wordpress.com/2018/02/openstackqueens-1.png) “人们希望从他们的云获得更多，”OpenStack 基金会首席运营官·马克·科利尔告诉我。这些用户希望在该平台上运行他们的传统工作负载和新工作负载，但是这些新工作负载的情况正在发生变化。“对我们来说，我们在新工作负载方面看到的是对机器学习的大量需求。这是一个非常热门的领域，人们很快就看到了其中的价值。”

因此，毫无疑问，Queens 版本中最引人注目的新特性之一是对 vGPUs 的内置支持，也就是说，将 GPU 附加到虚拟机的能力。

正如 Collier 和 OpenStack 执行董事 Jonathan Bryce 指出的那样，到目前为止，大多数用户都会选择运行带 GPU 的裸机服务器，但这也带来了设置这些机器的管理开销。现在，用户只需启动带有 vGPU 的虚拟机，就可以开始运行他们的科学和机器学习工作负载。

除了对 vGPUs 的支持，OpenStack 还增加了对其他硬件和软件加速资源的支持(想想 FPGAs、CryptoCards 等。)得益于新的 Cyborg 项目，它可以使这些资源作为独立的机器或作为核心 OpenStack 虚拟机平台的一部分或用于裸机部署。

不出所料，就像在公共云领域一样，各种 OpenStack 小组也在努力使容器成为平台更不可或缺的一部分。正如科利尔指出的那样，“一切都在继续集装箱化”。在这个版本中，这意味着新的 Zun container service for open stack 的推出，它允许用户轻松启动和运行容器，而不需要管理服务器和集群。使用一些核心 OpenStack 服务，Zun 处理运行这些容器所必需的网络、存储和认证。

Kuryr 项目也在这个版本中首次亮相，OpenStack 现在也增加了对 Kubernetes 的支持，Kubernetes 是容器编排的实际标准。Kuryr 将一些像[pod](https://web.archive.org/web/20221207212857/https://kubernetes.io/docs/concepts/workloads/pods/pod/)这样的 Kubernetes 本地概念引入 OpenStack 的网络堆栈中。

与此相关，OpenStack 项目也转向容器，将 OpenStack [带到网络的边缘](https://web.archive.org/web/20221207212857/https://www.openstack.org/edge-computing/)。一个新的项目，OpenStack-Helm，在 Kubernetes 之上为 OpenStack 提供了更简单的生命周期管理(并允许您作为独立的服务运行单独的 OpenStack 项目)，而另一个新的项目，LOCI，提供了这些服务的容器映像。这两个特性使得在边缘使用 OpenStack 变得更容易，尽管它们显然也有助于管理复杂的 OpenStack 部署。

正如科利尔和布莱斯所指出的，这个新版本为 OpenStack 增加了许多新的高可用性功能，这在很大程度上是对项目用户(包括从易贝到康卡斯特和深圳证券交易所的许多电信和大型企业)需求的反应。

OpenStack 团队仍在关注的一个新兴领域是无服务器计算。到目前为止，有一些社区项目正在探索这个领域，但是没有官方的无服务器 OpenStack 项目。布莱斯和科利尔告诉我，尽管如此，他们还是睁大了眼睛，认为许多新兴的开源无服务器框架已经主要依赖于 Kubernetes，这显然得到了该项目的全力支持。