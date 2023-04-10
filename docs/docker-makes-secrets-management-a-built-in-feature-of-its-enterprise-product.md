# Docker 将机密管理作为其企业产品 TechCrunch 的内置功能

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/09/docker-makes-secrets-management-a-built-in-feature-of-its-enterprise-product/>

# Docker 将机密管理作为其企业产品的内置功能

几年前，与使用虚拟机相比，使用[容器](https://web.archive.org/web/20221231043649/https://techcrunch.com/2016/10/16/wtf-is-a-container/)来运行您的应用程序会带来许多安全问题。随着企业开始以超出任何人预期的速度采用各种容器技术，这成为一个问题，像 Docker 这样的公司开始将安全性作为一个优先事项。尤其是对码头工人来说，这项工作开始有了回报。该公司今天[宣布](https://web.archive.org/web/20221231043649/https://blog.docker.com/2017/02/docker-datacenter-1-13/)它现在为 [Docker 数据中心](https://web.archive.org/web/20221231043649/https://www.docker.com/products/docker-datacenter)提供了一个[容器原生秘密管理解决方案](https://web.archive.org/web/20221231043649/https://blog.docker.com/2017/02/docker-secrets-management/)，允许开发者安全地将 API 密钥、加密密钥和密码提供给他们的应用程序，而不必使用第三方服务。

正如 Docker 安全主管 Nathan McCauley 告诉我的那样，共享这些秘密的传统方式通常包括将其复制到主机上，或者直接集成到源代码中。“容器颠覆了这一点，因为代码可以任意移动——甚至移动到不同的基础设施，”McCauley 说。因此，人们要么拼凑自己的解决方案，要么使用第三方服务，如 HashiCorp 的 [Vault](https://web.archive.org/web/20221231043649/https://www.vaultproject.io/) 。

[![937d1e2d-bf31-4875-a19c-3604d104dd89](img/d8066fe508c3bea3b0d006c954d1eb52.png)](https://web.archive.org/web/20221231043649/https://techcrunch.com/wp-content/uploads/2017/02/937d1e2d-bf31-4875-a19c-3604d104dd89.png)

McCauley 还抨击了 Docker 的容器编排竞争对手，认为简单地附加到这些工具上的解决方案本质上是不安全的。值得注意的是，Kubernetes 也有内置的工具来管理秘密。

Docker 的解决方案让您可以轻松地将秘密添加到您的集群(或者用 Docker 的说法是“蜂群”)中。它仅通过相互认证的 TLS 连接共享，然后安全地存储在管理器节点上，不会以不加密的方式写入磁盘。你可以在[这里](https://web.archive.org/web/20221231043649/https://docs.docker.com/engine/swarm/secrets/)找到一些例子来说明所有这些是如何在实践中发挥作用的。但是，这里的主要思想是确保所有这些都非常容易被开发人员集成，并且完全独立于底层基础设施。

正如 Docker 的企业营销副总裁 David Messina 告诉我的那样，该公司现在将安全性视为其主要卖点之一。他认为，该公司希望企业选择 Docker，因为它比其他选择(包括现有的遗留解决方案)更安全。“这是一英尺。我们一直拥有灵活性和便携性这两大支柱，这就是为什么每个人都被我们吸引，但我们宣布第三大支柱是安全性，”他补充道。