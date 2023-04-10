# 谷歌在 Docker 上押下重注，推出应用引擎集成、开源容器管理工具 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/06/10/google-bets-big-on-docker-with-app-engine-integration-open-source-container-management-tool/>

Docker 最近在开发者社区引起了轰动，谷歌也注意到了这一点。在[今年早些时候为计算引擎添加了](https://web.archive.org/web/20221209120138/http://docs.docker.com/installation/google/)一些基本的 Docker 支持后，该公司今天[宣布](https://web.archive.org/web/20221209120138/http://googlecloudplatform.blogspot.com/2014/06/an-update-on-container-support-on-google-cloud-platform.html)也将在应用引擎中采用 Docker，这得益于其最近推出的[托管虚拟机](https://web.archive.org/web/20221209120138/https://developers.google.com/cloud/managed-vms)。

为了帮助开发者使用 Docker，Google 今天也发布了一个管理容器的新工具 Kubernetes。为了巩固其在 Docker 社区的参与，该公司提名其基础设施副总裁 Eric Brewer 加入 Docker 治理委员会，“继续与社区合作，建立更好的开放容器标准。”

当然，容器对谷歌来说并不新鲜。在内部，该公司长期以来一直使用容器来管理其庞大的数据中心。事实上，它现在每周通过其数据中心发送超过 20 亿个集装箱。

![2014-06-10_0855](img/ef66c7140326faecfc087d50a16430c6.png)

谷歌产品经理 Craig McLuckie 曾领导公司在 Docker 上的大部分工作，他指出对 Docker 的支持对公司来说是理所当然的。在传统主机中，添加一个新的盒子总是一件大事。然而，现代应用程序通常被分解成许多微服务，容器非常适合这个世界。“对我们来说，集装箱提供了巨大的价值，”他告诉我。" Docker 为更多的开发者提供了很多这样的功能."

使用应用引擎上的 Docker，开发者可以访问已经存在的 Docker 图像的[大型库](https://web.archive.org/web/20221209120138/https://registry.hub.docker.com/)，或者他们可以通过谷歌的存储服务引入自己的图像。Docker 映像将部署在托管虚拟机中，这为应用引擎带来了很大的灵活性，因为它们允许开发人员运行谷歌平台即服务产品本身不支持的服务。

正如 McLuckie 告诉我的那样，该公司还希望让开发者能够非常容易地打包他们的 App Engine 应用程序，并从中创建 Docker 映像。

目前，应用引擎中的 Docker 支持仍处于测试阶段，想要尝试一下的开发者可以在这里[注册](https://web.archive.org/web/20221209120138/https://docs.google.com/a/google.com/forms/d/1_RfwC8LZU4CKe4vKq32x5xpEJI5QZ-j0ShGmZVv9cm4/viewform)。

一旦 Docker 开始运行，你就面临着管理和调度所有容器的挑战。这就是 Kubernetes 的用武之地(如果你想知道的话，它在希腊语中是“舵手”的意思)。Kubernetes 是一个开源的容器管理器，可以帮助您将容器部署到一组机器上。它提供了健康管理和复制功能，并使机器之间的连接变得更加容易。值得注意的是，容器管理器没有绑定到 Google 的服务，可以跨平台使用。

谷歌自己使用[欧米茄](https://web.archive.org/web/20221209120138/http://research.google.com/pubs/pub41684.html)作为其容器系统，但值得注意的是，虽然 Kubernetes 是建立在谷歌从运行其数据中心开发的专业知识上，但它是该公司专门为 Docker 编写的全新代码。这意味着比谷歌内部做的事情对开发者更友好(毕竟，大多数创业公司没有谷歌拥有的那种经验丰富的 DevOps 团队)。

根据 McLuckie 的说法，这个想法是为了让 Kubernetes 对大量开发人员来说是可接近的和可用的，这反过来将有助于将使用容器的想法带给更广泛的开发人员。代码现在可以在 GitHub 上获得。