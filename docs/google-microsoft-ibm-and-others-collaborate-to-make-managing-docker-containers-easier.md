# 谷歌、微软、IBM 和其他公司携手合作，让 Docker 容器的管理变得更加简单 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/07/10/google-microsoft-ibm-and-others-collaborate-to-make-managing-docker-containers-easier/>

# 谷歌、微软、IBM 和其他公司合作，使 Docker 容器的管理变得更加容易

这种支持者组合并不常见，但今天，[微软](https://web.archive.org/web/20230215190659/http://azure.microsoft.com/blog/2014/07/10/azure-collaboration-with-google-and-docker/)、[红帽](redhat.com)、 [IBM](https://web.archive.org/web/20230215190659/http://ibm.com/) 、 [Docker](https://web.archive.org/web/20230215190659/http://docker.io/) 、 [Mesosphere](https://web.archive.org/web/20230215190659/http://mesosphere.io/) 、 [CoreOS](https://web.archive.org/web/20230215190659/https://coreos.com/) 和 [SaltStack](https://web.archive.org/web/20230215190659/http://www.saltstack.com/) 联合起来支持[谷歌用于管理 Docker 容器的开源 Kubernetes 项目](https://web.archive.org/web/20230215190659/https://github.com/GoogleCloudPlatform/kubernetes)。

Docker 容器正迅速成为构建和运行分布式应用程序的首选技术。在过去的几个月里，每个主要的云供应商都支持 Docker 项目，Docker.io 最近在 B 轮融资中筹集了 1500 万美元，以继续扩展其平台服务。

尽管有这些支持，管理 Docker 容器有时仍然是一件麻烦事，所以一个月前， [Google](https://web.archive.org/web/20230215190659/http://www.crunchbase.com/organization/google) [基于其在自己的大规模数据中心使用容器的工作，推出了 Kubernetes 项目](https://web.archive.org/web/20230215190659/https://techcrunch.com/2014/06/10/google-bets-big-on-docker-with-app-engine-integration-open-source-container-management-tool/)。他们都将积极参与这些项目。

“每家公司都带来了独特的优势，我们将共同确保 Kubernetes 是一个强大和开放的容器管理框架，适用于任何应用程序和任何环境——无论是在私有、公共还是混合云，”谷歌高级副总裁 Urs hlz le 在今天的声明中说。

容器背后的想法是，开发者可以更容易地在不同的服务器和不同的云中部署和扩展他们的应用程序，所以[微软](https://web.archive.org/web/20230215190659/http://www.crunchbase.com/organization/microsoft)——或者[微软开放技术](https://web.archive.org/web/20230215190659/http://msopentech.com/blog/2014/07/10/bringing-new-open-source-container-technologies-microsoft-azure-google-docker/)，准确地说[——承诺](https://web.archive.org/web/20230215190659/http://azure.microsoft.com/blog/2014/07/10/azure-collaboration-with-google-and-docker/)它将在其 Azure 平台上的 Linux 环境中支持 Kubernetes。微软也将致力于支持另一个 Docker 支持的项目 [libswarm](https://web.archive.org/web/20230215190659/https://github.com/docker/libswarm) ，用于在 Azure 上构建网络服务。Docker 本身将致力于使 libswarm 与 Kubernetes 框架保持一致。

[Red Hat](https://web.archive.org/web/20230215190659/http://www.crunchbase.com/organization/red-hat) 承诺将 Kubernetes 引入其混合云，IBM[表示将为该项目和 Docker 生态系统贡献代码，“以确保容器是企业级的，并与社区合作围绕该项目创建一个开放的治理模型。”](https://web.archive.org/web/20230215190659/http://www.crunchbase.com/organization/ibm)

MesoSphere、CoreOS 和 SaltStack 将致力于将 Kubernetes 与他们自己的技术相结合。例如，[去年年底开始支持 Docker](https://web.archive.org/web/20230215190659/https://techcrunch.com/2013/09/26/mesosphere-adds-docker-support-to-its-mesos-based-operating-system-for-the-data-center/) 的 MesoSphere 将致力于将其调度和管理能力带给 Kubernetes 的客户。正如 CoreOS 团队告诉我的，Kubernetes 已经使用了 CoreOS 的 [etcd](https://web.archive.org/web/20230215190659/http://coreos.com/using-coreos/etcd/) 关键价值存储，它构成了 CoreOS 集群的主干。

总的来说，这似乎是 Docker 项目的好消息。Kubernetes 支持者名单上的每个人之前都以某种形式支持 Docker，但让这群公司在 Docker 生态系统中合作只会有助于它的采用(从长远来看，可能会给其他虚拟化技术带来麻烦)。