# Istio 服务网推出 1.0 版 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/07/31/the-open-source-istio-service-mesh-for-microservices-hits-version-1-0/>

来自 Google、IBM、Lyft、Red Hat 和开源社区中许多其他参与者的微服务的服务网格,[今天发布了其工具的 1.0 版本](https://web.archive.org/web/20221207213214/https://istio.io/blog/2018/announcing-1.0/)。

如果你[不喜欢服务网](https://web.archive.org/web/20221207213214/https://thenewstack.io/history-service-mesh/)，这是可以理解的。很少有人是。但是 Istio 可能是目前最重要的新开源项目之一。它位于许多行业趋势的交汇点，如容器、微服务和无服务器计算，并使企业更容易接受它们。Istio 现在有 200 多个贡献者，自 0.1 版本推出以来，代码已经有 4000 多次签入。

Istio，[的核心](https://web.archive.org/web/20221207213214/https://istio.io/docs/concepts/what-is-istio/)，处理微服务的路由、负载平衡、流量控制和安全需求。它位于现有分布式应用程序之上，基本上帮助它们安全地相互对话，同时还提供日志记录、遥测和必要的策略，使事情处于控制之下(并且安全)。它还支持 canary 版本，允许开发者在向更广泛的受众发布更新之前，先在少数用户中测试更新，这是谷歌和其他 webscale 公司长期以来在内部做的事情。

![](img/d53383dd39ea4df77135a6c3d7866ec3.png)“在区的微服务 、 事 事 动 所以 很快，”谷歌产品经理詹妮弗·林告诉我。随着的成功Kubernetes围绕容器 编排 的抽象， Istio 被 形成了 作为打开-  来源 项目 到 真的 取下一步中的 术语  基础 工作量 到 移动 成 更多的 一  服务 管理 层 。  所以 真的是围绕正确的抽象层次 为 服务 和 创建一个一致的 环境

甚至在 1.0 版本发布之前，许多公司已经在生产中采用了 Istio，包括易贝和英国汽车贸易商。林认为，这是一个迹象，表明 Istio 解决了许多企业在采用微服务时面临的问题。“许多更成熟的客户试图构建他们自己的服务管理层，虽然我们还没有宣布 1.0，但我们努力让许多客户(包括数量惊人的大型企业客户)说，‘你知道，即使你不是 1.0，我也很乐意将它投入生产，因为我与之相比要原始得多。’"

IBM 研究员兼云计算副总裁 Jason McGee 同意这一点，并指出“自 Istio 推出以来，我们的使命就是让每个人都能通过微服务取得成功，尤其是在企业中。这就是为什么我们将社区的重点放在提高安全性和可扩展性上，并在很大程度上依靠我们从为各种规模的公司构建敏捷云架构中学到的东西。"

许多大型云玩家现在也直接支持 Istio。例如，IBM 在其 Kubernetes 服务的基础上支持它，谷歌甚至为其谷歌云用户宣布了一项由[管理的 Istio 服务](https://web.archive.org/web/20221207213214/https://cloudplatform.googleblog.com/2018/07/cloud-services-platform-bringing-the-best-of-the-cloud-to-you.html)，以及一些用于基于 Kubernetes 和 Istio 的无服务器应用的[额外开源工具](https://web.archive.org/web/20221207213214/https://cloud.google.com/knative/)。

今天的聚会少了两个名字，微软和亚马逊。不过，如果这个项目保持势头，我认为这种情况会随着时间的推移而改变。

Istio 也没有加入任何主要的开源基金会。Kubernetes 的家乡云原生计算基金会(CNCF)正在支持 linkerd，这是一个与 Istio 没有什么不同的项目。一旦这类项目的 1.0 版本推出，维护人员通常会开始寻找一个可以指导项目开发的基础。我猜我们听到更多关于 Istio 将在哪里着陆的消息只是时间问题。