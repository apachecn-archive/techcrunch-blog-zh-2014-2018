# 微软 Azure 容器服务上的 Kubernetes 现已全面上市 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/21/kubernetes-on-microsofts-azure-container-service-is-now-generally-available/>

# 微软 Azure 容器服务上的 Kubernetes 现在已经普遍可用

Kubernetes，Google 孵化的开源容器编排系统，正在迅速成为管理大型容器部署的事实上的标准。去年，微软在其 Azure 容器服务中推出了对 Kubernetes 支持的预览版；今天，它把这项服务从测试版中拿出来，并使其普遍可用。

这意味着服务现在由 SLA 支持，用户将能够从微软获得支持合同。不过，也许更重要的是，微软在这次更新中还增加了两个关键的新功能:轻松扩展 Kubernetes 集群的能力，以及支持多主机的高可用性设置。

在预览版中，正如微软合作伙伴架构师(Kubernetes 项目的联合创始人)Brendan Burns 告诉我的那样，用户只能建立一个集群并测试它，但如果他们想让它变大或变小，他们就必须拆除它。你可能会认为易于扩展是使用容器编排服务的主要原因之一，但 Burns 认为这仍然是一个预览，该公司并不希望用户在生产中运行它(尽管有些人这样做了)。

该团队还在 Kubernetes 本身做了大量工作，以添加对 Windows Server 容器的支持，这使得 Windows 用户可以打包他们的容器，然后可以在 Windows Server 2016 上运行。通过此次更新，Azure 容器服务上的 Kubernetes 现在支持预览版中的 Windows Server 容器。伯恩斯说，该公司已经看到了很多人对这一功能的兴趣。“我认为这反映了一个事实，即这些容器化的工作流提高了开发人员的工作效率，无论他们是新的应用程序还是您为 Windows Server Containers 打包的现有应用程序。”

伯恩斯还指出，该团队改进了在 Azure 容器服务上使用 Kubernetes 的命令行支持。此外，该团队将其对中间层 DC/操作系统的支持更新至最新版本。

Burns 今天在[集装箱世界](https://web.archive.org/web/20221206060328/https://tmt.knect365.com/container-world/)演讲，他给了我一个简短的预览。归根结底，容器已经成为主流。“一直以来，集装箱基础设施的概念是值得关注的，但现在它只是基础设施，”他告诉我。他认为，集装箱快速增长的原因是它解决了很多问题——而且速度很快。“无论你在做什么，这种变化对你都有好处，特别是如果你不仅可以忘记物理硬件，还可以忘记虚拟机，”他说。