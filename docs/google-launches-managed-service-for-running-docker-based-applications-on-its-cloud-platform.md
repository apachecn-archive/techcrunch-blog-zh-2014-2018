# 谷歌推出托管服务，在其云平台 TechCrunch 上运行基于 Docker 的应用程序

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/11/04/google-launches-managed-service-for-running-docker-based-applications-on-its-cloud-platform/>

# 谷歌推出托管服务，在其云平台上运行基于 Docker 的应用程序

Google today [宣布](https://web.archive.org/web/20221206060756/http://googlecloudplatform.blogspot.fr/2014/11/google-cloud-platform-live-introducing-container-engine-cloud-networking-and-much-more.html)Google Container Engine 的 alpha 发布，这是一个新的托管服务，用于在其云平台上构建和运行基于 Docker 容器的应用程序。

[Docker](https://web.archive.org/web/20221206060756/https://www.docker.com/) 可能是最近开发人员圈子里最热门的技术——几乎不可能不提到它就与开发人员进行讨论——谷歌的云平台团队已经决定全力以赴[开发这项让开发人员更容易运行分布式应用的技术。](https://web.archive.org/web/20221206060756/https://beta.techcrunch.com/2014/06/10/google-bets-big-on-docker-with-app-engine-integration-open-source-container-management-tool/)

本质上，这项新服务是一个基于谷歌开源项目的“集群即服务”平台。Kubernetes 帮助开发人员管理他们的容器集群，它是基于谷歌自己在其大规模数据中心对容器的工作。在这个新服务中，Kubernetes 动态地管理不同的 Docker 容器，这些容器为用户组成了一个应用程序。

谷歌表示，“快速启动、高效虚拟机主机和无缝虚拟化网络集成”的结合将使其云计算服务成为“运行基于容器的应用程序的最佳场所。”该公司的竞争对手可能会反驳这一点，但在这一点上他们都没有提供类似的服务。

谷歌最初在 5 月推出了对 Docker 镜像的支持，作为其新的[托管虚拟机服务](https://web.archive.org/web/20221206060756/https://beta.techcrunch.com/2014/03/25/google-launches-managed-virtual-machines-gives-developers-a-middle-ground-between-compute-and-app-engine/)的一部分。这些受管理的虚拟机来自谷歌有限的 alpha，增加了自动扩展支持，因此开发人员现在可以在谷歌的平台上使用 Docker 容器，而不必经历任何困难。不过，托管虚拟机目前仍处于测试阶段，在谷歌的新语言中，这意味着没有访问控制，费用可能会被免除，但也没有 SLA 或技术支持义务。

请记住，因为这项新服务还处于正式发布阶段，它的功能还不完整，整个基础设施随时都可能崩溃。