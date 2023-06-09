# 圣何塞 Strata + Hadoop World 2016 上值得关注的七件事 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/03/29/seven-things-to-watch-for-at-strata-hadoop-world-2016-in-san-jose/>

[Josh Klahr](https://web.archive.org/web/20230131001426/https://www.crunchbase.com/person/josh-klahr#/entity)

是 Atscale 的产品副总裁。

随着 Strata + Hadoop World 的启动，退一步看看会议的内容，以此了解大数据世界正在发生的事情，总是令人着迷。

对于那些参加这个会议已经超过五年的人来说，你可能已经看到它从一个软件开发人员试验开源技术的舞台转变为一个更重要的企业软件会议——在这个会议上，开发人员、高管、供应商和专业服务提供商聚集在一起，分享和了解该领域的最新发展。

为了快速找出今年圣何塞会议上的“热点”,我对一周内出现在培训课程、主题演讲和演示会议列表中的热门术语进行了快速(且极不科学)的分析。在过滤掉显而易见的术语(Hadoop、数据、分析、Apache)后，一些清晰的主题出现在顶部，如下所示:

![pasted image 0 (10)](img/49dc6c19cb8e9343ca7c508936e3b5a0.png)

在查看了这一特定的数据视图后，有几个关键的东西跳了出来，我怀疑这些数据表明了整个行业正在发生的关键趋势。

**Spark 的采用和兴趣持续增长:**虽然 Hadoop 的采用仍有几年的时间，但 Spark 在大数据生态系统中的增长非常显著。这两种技术都将继续存在，Spark 被广泛用于各种用例，包括流水线数据处理和可并行化的数据科学工作负载。

**流媒体和实时是“下一个大事件”:**在上面的图表中，你会看到像“流媒体”和“实时”这样的术语，以及“卡夫卡”和“融合”(卡夫卡的商业发行版)。现在，企业已经成功地在生产 Hadoop 集群中批量加载和处理数据，人们越来越关注实时数据接收、处理和分析。

**可视化仍然很重要:**正如 [AtScale 的 Hadoop 成熟度调查](https://web.archive.org/web/20230131001426/http://www.forbes.com/sites/gilpress/2015/09/17/5-highlights-of-the-first-and-largest-hadoop-maturity-survey-released-today/#50c5b5bd7704)所揭示的，在投资数据科学之前，企业更关注在 Hadoop 上推出商业智能用例(尽管媒体持续断言[数据科学有多性感](https://web.archive.org/web/20230131001426/https://hbr.org/2012/10/data-scientist-the-sexiest-job-of-the-21st-century/))。数据可视化和自助服务仍然是一个关键的投资领域，即使在 Hadoop 领域也是如此。

**SQL-on-Hadoop 已经成为主流:**值得注意的是，Hadoop 世界的热门术语和主题中缺少 SQL-on-Hadoop。前几年，从 Hive 开始，到像 Impala 和 SparkSQL(以及许多其他基于 Hadoop 的商业 SQL 产品)这样的项目，人们对这些技术非常关注。但是 SQL-on-Hadoop 已经成为 Hadoop 工具包中的“必备”，并且已经进入主流。正如我们最近的 [BI-on-Hadoop 基准](https://web.archive.org/web/20230131001426/http://blog.atscale.com/how-different-sql-on-hadoop-engines-satisfy-bi-workloads)所揭示的，这些引擎现在已经准备好支持大规模的分析性 SQL 工作负载。

**在内存基板方面…下一步的优化？:**一个有趣的项目是“alluxio”，这是最近更名的超光速粒子项目。Alluxio 是一个虚拟分布式存储系统，它具有以内存为中心的架构，能够以内存速度跨集群共享数据。对于 Hadoop 上的 SQL 引擎，这意味着更快的查询时间和更高的性能，正如百度所经历的那样，他们采用 Alluxio 来加速他们的分析数据处理。

**Hadoop 的采用仍然是人们的首选:“采用”和“生产”位列其中:**许多 IT 组织在 Hadoop 上押下了重注，将其作为下一代数据平台，并将工作负载从 Teradata 等传统系统迁移到成本更低、可扩展性更强的环境中。对于这些组织来说，展示他们的 Hadoop 投资以生产集群的形式获得回报是至关重要的，这些生产集群被核心业务功能(如商业智能)所采用。

**不要忽视云中的大数据:**亚马逊和微软都出现在名单上。尽管在 Hadoop 领域起步缓慢，但微软正在大数据领域取得重大进展，提供了 HDInsight(可在 Linux 上运行！).亚马逊继续在大数据产品方面取得长足进步，不断增加的红移采用补充了 S3 和 EMR(弹性 MapReduce)等已经流行的服务。