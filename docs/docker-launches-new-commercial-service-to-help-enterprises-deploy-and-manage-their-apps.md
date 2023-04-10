# Docker 推出新的商业服务，帮助企业部署和管理其应用程序 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/11/17/docker-launches-new-commercial-service-to-help-enterprises-deploy-and-manage-their-apps/>

Docker 今天在巴塞罗纳开发者大会上宣布了 Docker 通用控制平面(UCP)。UCP 是 Docker 产品组合中的一项新的付费服务，旨在帮助运营团队轻松建立集群，并使开发人员能够在其上部署 Docker 化的应用。

根据 Docker 的产品副总裁 Scott Johnston 的说法，开发人员(他们只想开始采用 Docker 和其他新技术)与负责保护公司基础设施安全和可靠性的 IT 运营团队之间一直存在一些紧张关系。通常，这意味着必须做出权衡，因为很难同时确保速度和安全性。

使用新工具，企业将能够使用基本的图形界面和标准的 Docker 命令行工具为开发人员提供他们想要的自助服务选项，同时 IT 部门能够部署和管理基础架构。

【T2![docker_control_plane_schematics](img/d83b3614649d4384ccfdb74ede1d66cc.png)

正如 Johnston 指出的，该产品建立在现有工具的基础上，如 Docker-native 集群管理器 Docker Swarm、Docker Engine、Docker Compose 和其他标准工具。然而，除此之外，该团队还添加了许多企业需要的控制功能。例如，UCP 集成了现有的 LDAP 和 Active Directory 安装，并允许管理员控制对特定集群、应用程序、容器和映像的访问。

同样，该服务提供用户审计日志，并提供开箱即用的 TLS 支持。管理员和用户还可以获得一套基本的集群图形监控工具。

企业在其场所部署 UCP，但该服务可以控制本地集群和公共云中的集群。原因是该服务全面使用标准的 Docker APIs，这将使已经熟悉 Docker 的开发人员非常容易使用。

同时，这也意味着该服务可以扩展到 Docker 生态系统中几乎所有现有的服务。例如，如果您需要更复杂的监控解决方案，现有的服务可以直接插入您的 UCP 集群。

[![tutum_ucp](img/bc5922adb9d4b184321d6fff118b9769.png)](https://web.archive.org/web/20221007114825/https://beta.techcrunch.com/wp-content/uploads/2015/11/tutum_ups.png)

在许多方面，UCP 是本地企业版的 [Tutum](https://web.archive.org/web/20221007114825/https://www.tutum.co/) ，这是一个基于云的服务，用于部署和管理 Docker [上个月](https://web.archive.org/web/20221007114825/https://blog.docker.com/2015/10/docker-acquires-tutum/)收购的 Docker 应用。

UCP 现在是私人测试版(你可以在这里注册)。Docker 尚未宣布任何定价，也不清楚 UCP 将于何时全面上市。

【T2![control_plane_2](img/04280c70d167b76bf15937317f58a07f.png)