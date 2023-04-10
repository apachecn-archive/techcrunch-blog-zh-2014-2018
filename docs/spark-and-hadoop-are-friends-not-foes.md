# Spark 和 Hadoop 是朋友，而不是敌人

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/07/12/spark-and-hadoop-are-friends-not-foes/>

六月对于阿帕奇 Spark 来说是激动人心的一个月。在圣何塞 Hadoop 峰会上，这是一个经常谈论的话题，也是许多会议演示的主题。6 月 15 日，IBM 宣布计划对 Spark 相关技术进行大规模投资。

这一声明帮助启动了在三藩市举行的 [Spark 峰会](https://web.archive.org/web/20230320090507/https://spark-summit.org/2015/)，在那里可以看到越来越多的工程师了解 Spark——以及越来越多的公司尝试和采用 Spark。

Spark 投资和采用的良性循环正在快速推动这一重要技术的成熟和能力，使整个大数据社区受益。然而，对 Spark 越来越多的关注也引发了一个奇怪而顽固的误解:Spark 在某种程度上是 Apache Hadoop 的*替代品*，而不是它的补充。这种误解可以在标题中看到，如[“新软件旨在处理 Hadoop 的数据”](https://web.archive.org/web/20230320090507/http://www.wsj.com/articles/newer-software-aims-to-crunch-hadoops-numbers-1434326008?KEYWORDS=spark+dwoskin)和[“公司从大数据技术 Hadoop 转移。”](https://web.archive.org/web/20230320090507/http://bits.blogs.nytimes.com/2015/06/15/companies-are-moving-on-from-big-data-technology-hadoop/?_r=1)

作为一个长期的大数据从业者，雅虎投资 Hadoop 的早期倡导者！现在，我是一家为企业提供大数据即服务的公司的首席执行官，我想为这次对话带来一些观点和清晰性。

Spark 和 Hadoop 协同工作。

Hadoop 日益成为大数据的首选企业平台。Spark 是一种运行在 Hadoop 之上的内存处理解决方案。Hadoop 的最大用户——包括易贝和雅虎！—两者都在其 Hadoop 集群中运行 Spark。Cloudera 和 Hortonworks 将 Spark 作为其 Hadoop 发行版的一部分。自从我们发布以来，Altiscale 的客户一直在 Hadoop 上使用 Spark。

将 Spark 定位于 Hadoop 的对立面，就好比说你的新电动汽车太酷了，你再也不需要电了。如果有什么不同的话，电动汽车将推动对更多电力的需求。

为什么会困惑？现代 Hadoop 由两个主要组件组成。第一个是名为 Hadoop 分布式文件系统(HDFS)的大规模存储系统，它以低成本、高性能的方式存储数据，并针对大数据的数量、种类和速度进行了优化。第二个组件是一个名为 YARN 的计算引擎，它可以在存储在 HDFS 的数据上运行大规模并行程序。

YARN 可以托管任意数量的编程框架。最初的此类框架是 MapReduce，由谷歌发明，用于帮助处理大量的网络抓取。Spark 是另一个这样的框架，另一个叫做 Tez 的新框架也是如此。当人们谈论 Spark“碾压”Hadoop 时，他们真正的意思是程序员现在更喜欢使用 Spark 而不是旧的 MapReduce 框架。

但是，MapReduce 不应该等同于 Hadoop。MapReduce 只是在 Hadoop 集群中处理数据的众多方法之一。Spark 可以作为替代。更广泛地看，业务分析师——大数据从业者的基础越来越大——避免使用这两种框架，它们是面向程序员的低级工具包。相反，他们使用像 SQL 这样的高级语言，使 Hadoop 更容易访问。

在过去四年中，基于 Hadoop 的大数据技术出现了前所未有的创新水平。我们已经从批处理 SQL 发展到了交互式 SQL 从一个框架(MapReduce)到多个框架(例如 MapReduce、Spark 等等)。

我们在 HDFS 看到了巨大的性能和安全性改进，我们也看到了基于所有这些的工具的爆炸式增长，如 [Datameer](https://web.archive.org/web/20230320090507/http://www.datameer.com/) 、 [H20](https://web.archive.org/web/20230320090507/http://h2o.ai/) 和 [Tableau](https://web.archive.org/web/20230320090507/http://www.tableau.com/) ，这些工具使所有这些大数据基础设施可供更广泛的数据科学家和业务用户使用。

Spark 不是将取代 Hadoop 的挑战者。相反，Hadoop 是让 Spark 成为可能的基础。随着组织寻求最广泛、最强大的平台来将其数据资产转化为可操作的业务洞察力，我们预计这两者的采用率将会越来越高。