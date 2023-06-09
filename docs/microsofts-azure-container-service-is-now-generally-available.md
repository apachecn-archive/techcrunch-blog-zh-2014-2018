# 微软的 Azure 容器服务现已正式推出 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/04/19/microsofts-azure-container-service-is-now-generally-available/>

微软为其 Azure 云计算服务提供的容器调度和协调服务 Azure Container Service 现已正式推出。

这项服务允许用户选择 Mesosphere 的[数据中心操作系统](https://web.archive.org/web/20221207181747/https://dcos.io/) (DC/OS)或 Docker 的 [Swarm and Compose](https://web.archive.org/web/20221207181747/https://blog.docker.com/2015/02/orchestrating-docker-with-machine-swarm-and-compose/) 来部署和编排他们的容器，于 2015 年 9 月首次宣布，并于今年 2 月进行了公开预览。

正如微软的 Azure 首席技术官(兼临时小说家)马克·鲁西诺维奇告诉我的，他认为这种使用 Docker Swarm/Compose 和 DC/OS 的开源组件的能力让 Azure Container 服务从一些竞争对手中脱颖而出。

正如 Russinovich 告诉我的，该公司不想告诉其客户使用这两种服务中的哪一种。“我们的工作是确保我们的客户可以在我们的云上使用其中一个或两个，并获得良好的体验，”他说。

当然，微软在中间层的历史可以追溯到很久以前。起初，该公司与 Mesosphere 合作，允许其用户在 Azure 上运行其 DC/操作系统；两家公司还合作将 DC/操作系统支持引入 Windows 和 Hyper-V 容器。此外，微软对公司进行了[战略投资(据报道，微软](https://web.archive.org/web/20221207181747/http://hewlettpackardventures.com/mesosphere-raises-73-5-million-in-series-c-funding/)[去年一度试图收购 Mesosphere，当然，Russinovich 不想对此发表评论)。](https://web.archive.org/web/20221207181747/https://www.theinformation.com/microsoft-has-been-in-buyout-talks-with-mesosphere)

微软还认为，使用这些开源解决方案意味着其用户可以在需要时轻松地将工作负载转移到本地(当然，也可以将现有的本地解决方案转移到 Azure)。

然而，微软的产品线中缺少的一项服务是谷歌的 Kubernetes，这也是一个开源项目。Russinovich 认为，该公司正专注于其客户所要求的开源技术——他显然暗示，其客户目前并没有要求 Kubernetes(尽管他也保留了 Azure Container Serviceswould 有一天会支持它的可能性)。

正如 Russinovich 指出的，该公司看到许多公司正在将他们的工作负载转移到容器上。“几年前，它主要是开发测试，但现在整个公司都在生产中采用它，”他说。

Russinovich 告诉我，微软目前没有任何计划通过目前与 Red Hat 的类似安排提供支持，例如，Red Hat 和微软的员工在同一地点。微软将提供基本的中间层支持，中间层将处理高级主题的 2/3 层支持。

[https://web.archive.org/web/20221207181747if_/https://www.youtube.com/embed/7PUtVXtiLD4?feature=oembed](https://web.archive.org/web/20221207181747if_/https://www.youtube.com/embed/7PUtVXtiLD4?feature=oembed)

视频