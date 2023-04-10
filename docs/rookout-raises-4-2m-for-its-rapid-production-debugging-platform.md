# Rookout 为其快速生产调试平台 TechCrunch 筹集了 420 万美元

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/04/25/rookout-raises-4-2m-for-its-rapid-production-debugging-platform/>

很少有人因为喜欢调试而从事编码工作，但是因为没有完美的代码，问题不可避免地会出现。以色列初创公司 [Rookout](https://web.archive.org/web/20221204121551/https://www.rookout.com/) 正在解决这个问题的一个方面，它帮助开发人员跟踪生产代码中的问题，而不强迫开发人员编写任何额外的代码来编写额外的测试和重新部署他们的应用程序。正如该公司今天宣布的那样，它已经从 TLV 合伙人和 Emerge 获得了 420 万美元的种子资金。

Rookout 联合创始人 Or Weis 和 Liran Haimovitch 告诉我，他们自己编写代码的经验导致他们开始了这个项目。Weis 担任首席执行官，Haimovitch 担任首席技术官，他指出，就在几年前，你的代码将在自己的盒子中运行，你可以完全控制它。然而，现在你的代码可能在多个位置运行，几乎不可能访问应用程序的整个状态。因此，当产品中出现 bug 时——尽管在开发过程中进行了所有的测试，但它们经常出现——调试就成了一个真正的痛点。

https://youtu.be/qTdpOC92DBI

Rookout 对此的解决方案是用“不会中断的断点”来检测代码。要做到这一点，你需要将 Rookout 的在线 IDE 与你在 GitHub、Bitbucket 或其他 git 托管服务上的代码库连接起来(或者与你的本地文件系统连接起来)。IDE 将获取代码并让您浏览它。开发人员通常有一种直觉，知道错误可能在哪里，所以当您到达可疑文件时，您可以使用 Rookout 的可视化规则编辑器来设置虚拟断点。一旦生产代码再次运行，所有的数据都会自动推入 IDE，以便您可以检查整个堆栈跟踪，直到您设置断点的位置。

所有这些都适用于用 Python 和 Node.js 编写的代码，以及像 Scala 或 Kotlin 这样的 Java 虚拟机(JVM)语言。至于环境，该服务目前适用于部署在 AWS、Azure、谷歌云和本地服务器上的代码，也可以用于无服务器和容器化的应用程序。

虽然 Rookout 专注于收集数据，但团队非常清楚 Rookout 不想成为应用程序性能监控工具这一事实。但是，您可以将您的 Rookout 数据转发给这些工具。

韦斯和海莫维奇告诉我，该公司现在有 14 名员工和“几十个”客户。展望未来，该团队计划在收到请求时添加对 Go 和其他语言的支持，并逐渐添加更多的 IDE 支持。

像许多创业公司一样，创始人仍在研究他们的定价模式。目前的计划是围绕一家公司正在使用的主机数量，尽管这仍有可能发生变化。

[https://web.archive.org/web/20221204121551if_/https://www.youtube.com/embed/pzd8oTYRS6U?feature=oembed](https://web.archive.org/web/20221204121551if_/https://www.youtube.com/embed/pzd8oTYRS6U?feature=oembed)

视频