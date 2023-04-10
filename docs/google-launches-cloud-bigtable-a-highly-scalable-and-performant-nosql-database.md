# Google 推出云 Bigtable，这是一个高度可扩展和高性能的 NoSQL 数据库 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/05/06/google-launches-cloud-bigtable-a-highly-scalable-and-performant-nosql-database/>

# 谷歌推出云大表，一个高度可扩展和高性能的 NoSQL 数据库

借助云 Bigtable，谷歌今天推出了新的 NoSQL 数据库产品，顾名思义，该产品由该公司的 Bigtable 数据存储系统提供支持，但增加了一点，即它与 [Apache HBase API](https://web.archive.org/web/20221209134013/http://hbase.apache.org/) 兼容，后者本身基于谷歌的 [Bigtable 项目](https://web.archive.org/web/20221209134013/http://research.google.com/archive/bigtable.html)。Bigtable 为 Gmail、Google Search 和 Google Analytics 等提供支持，因此这绝对是一项久经考验的服务

谷歌承诺，与 HBase 和 Cassandra 等公司相比，云 Bigtable 将提供个位数的毫秒延迟和 2 倍的性能。由于支持 HBase API，Cloud Bigtable 可以与 Hadoop 生态系统中所有现有的应用集成，但它也支持 Google 的[云数据流](https://web.archive.org/web/20221209134013/https://cloud.google.com/dataflow/)。

设置一个云 Bigtable 集群应该只需要几秒钟，存储会根据用户的需求自动扩展。

值得注意的是，这并不是谷歌的第一个基于云的 NoSQL 数据库产品。通过[云数据存储](https://web.archive.org/web/20221209134013/https://cloud.google.com/datastore/docs/concepts/overview)，谷歌已经在其应用引擎平台上为开发者提供了高可用性的 NoSQL 数据存储。该服务也是基于 Bigtable 的。谷歌云平台产品经理科里·奥康纳(Cory O'Connor)告诉我，云数据存储侧重于 web 应用程序和移动应用程序的读密集型工作负载。

“云 Bigtable 恰恰相反，它是为需要大量数据处理并且工作负载更加复杂的大型公司和企业而设计的，”O'Conner 告诉我。“例如，如果组织需要大规模地将数据流入单个数据库、在单个数据库上运行分析以及从单个数据库提供数据，那么云 Bigtable 就是合适的系统。我们的许多客户将从云数据存储开始构建原型并快速移动，然后随着他们的增长和他们的数据处理需求变得更加复杂，向云 Bigtable 等服务发展。”

这项新服务现在处于测试阶段，这意味着它对所有开发者开放，但不提供 SLA 或技术支持。