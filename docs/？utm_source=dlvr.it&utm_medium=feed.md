# 谷歌为云平台用户推出私人 Docker 仓库

> 原文：<https://web.archive.org/web/http://techcrunch.com/2015/01/23/google-docker-repository/?utm_source=dlvr.it&utm_medium=feed>

# 谷歌为云平台用户推出私人 Docker 仓库

谷歌今天[宣布](https://web.archive.org/web/20230313170547/http://googlecloudplatform.blogspot.com/2015/01/secure-hosting-of-private-Docker-repositories-in-Google-Cloud-Platform.html)为其云平台推出[谷歌容器注册表](https://web.archive.org/web/20230313170547/https://cloud.google.com/tools/container-registry/)的测试版。这项新服务允许开发人员在公司的云计算平台上托管、共享和管理他们的私有 Docker 容器库。

默认情况下，Docker 提供了自己的[公共图像注册表](https://web.archive.org/web/20230313170547/https://registry.hub.docker.com/)，这样开发者可以快速安装任何东西，从一台基本的未经修饰的 Ubuntu 机器到已经设置好运行 WordPress、mongoDB、Hadoop 或几乎任何你能想到的其他服务器包的服务器。当然，许多企业没有兴趣将其容器发布到公共存储库中。他们可以运行自己的私有存储库，或者使用像 Quay.io 这样的服务，这些服务以云服务的形式提供这一功能。在其核心，这也是谷歌的容器注册所做的，但重点是谷歌自己的云计算平台。

与所有处于测试阶段的谷歌云平台项目一样，容器注册表目前是免费的，对所有开发者开放。

以下是谷歌所说的使用其系统的优势:

*   **访问控制**:注册服务将你的私人图像托管在你的谷歌云平台项目下的[谷歌云存储](https://web.archive.org/web/20230313170547/https://cloud.google.com/storage/)中。这确保了默认情况下您的私有图像只能由您的项目成员访问，使他们能够通过 [Google Cloud SDK](https://web.archive.org/web/20230313170547/https://cloud.google.com/sdk/) 命令行安全地推送和提取图像。然后，容器主机虚拟机可以轻松访问安全的映像。
*   **服务器端加密**:您的私人图像在写入磁盘之前会自动[加密](https://web.archive.org/web/20230313170547/https://cloud.google.com/storage/docs/concepts-techniques#encryption)。
*   **快速可靠的部署**:您的私人图像存储在谷歌云存储中，并缓存在我们的数据中心，随时准备通过谷歌云平台的[仙女座号网络结构](https://web.archive.org/web/20230313170547/http://googlecloudplatform.blogspot.com/2014/11/cloud-networking-more-connectivity-choices-better-performance-and-lower-prices.html)部署到谷歌容器引擎[集群](https://web.archive.org/web/20230313170547/https://cloud.google.com/container-engine/docs/clusters/)或谷歌计算引擎[容器优化虚拟机](https://web.archive.org/web/20230313170547/https://cloud.google.com/compute/docs/containers/container_vms)。

谷歌在 Docker 上下了一个早期赌注，可能是因为它也一直将容器作为自己基础设施的核心功能。例如，它在开源项目上投入了大量资金，比如 Kubernetes，并且在去年 11 月推出了专用的容器引擎服务。

值得注意的是，亚马逊[在去年 11 月](https://web.archive.org/web/20230313170547/https://techcrunch.com/2014/11/13/amazon-announces-ec2-container-service-for-managing-docker-containers-on-aws/)推出了其 EC2 容器服务[。虽然开发者可以将它与任何第三方 Docker 注册表一起使用，但亚马逊本身目前并不提供注册表服务。](https://web.archive.org/web/20230313170547/http://cts.businesswire.com/ct/CT?id=smartlink&url=https%3A%2F%2Faws.amazon.com%2Fecs&esheet=50983802&newsitemid=20141113006305&lan=en-US&anchor=https%3A%2F%2Faws.amazon.com%2Fecs&index=1&md5=f86e73492f95bfe9fd630de69d22ebff)