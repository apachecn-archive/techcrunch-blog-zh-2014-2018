# 分析年度

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/01/15/the-year-in-analytics-2/>

萨米尔·萨克兰撰稿人

Sameer Al-Sakran 是

[Metabase](https://web.archive.org/web/20230326022526/http://www.metabase.com/)

，一家开源商业智能公司。

More posts by this contributor

好了，2016 年正式过去了。在选举大戏、股票市场的辗转反侧、名人的继续前进和哈兰贝之间，这是一件非常美妙的事情。

## SaaS 修正

首先要做的事情。如果不考虑 2 月份 SaaS 倍数暴跌的情况，很难理解分析生态系统的整体状况。大多数老练的观察家已经认识到这样一个事实:一家处于高速增长模式的 SaaS 公司会吃掉每一块钱，甚至更多。然而，除非你能获得非常精细的客户获取成本、客户流失率和群体活动数据，否则很难区分一家健康高速增长的 SaaS 公司和一家为低质量增长付出过高代价的公司。

你友好的邻居 SaaS 的首席财务官不太可能在他们的 10-q 中包含这种精细粒度的数据。这一点，再加上大量现金被烧掉，使得投资者在经济增长似乎放缓时非常焦虑。 [LinkedIn](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/02/04/linkedin-tumbles-24-on-earnings-guidance/) 在 2016 年也有过这样的[不幸时刻](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/02/23/linkedin-problems-run-deeper-than-valuation/)，并在 2 月初成功毁掉了很多其他公司的夜晚。Tableau、Qlik、Salesforce 和许多其他公司受到的打击尤其严重。

## 数据仓库的现状

我们将从数据仓库世界在 2016 年发生的变化开始。数据仓库是存储数据的地方；它们支持分析用途。除非您使用一体化云 BI 提供商(如 Domo、GoodData 等。)，数据仓库是任何分析基础架构的核心组件。2016 年，我们在 2015 年注意到的主要趋势[](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/01/09/the-year-in-analytics/)—基于 Hadoop 的 SQL 取代传统的分析数据库，并将数据仓库整合到云托管提供商产品中——仍在继续。

## Hadoop 上的 SQL

从早期开始，Hadoop 就被广泛用于商业智能和分析用例，即使它不是 it 的最佳选择。2016 年，各种基于 Hadoop 的 SQL 选项开始排挤其他分析数据仓库。

主要项目(蜂巢、黑斑羚、普雷斯托和火花)都有显著提高性能和稳定性的主要版本。 [Hive](https://web.archive.org/web/20230326022526/http://blog.cloudera.com/blog/2016/03/apache-hive-2-0-is-released/) ，最初的 Hadoop 上的 SQL 播放器，在三月份发布了一个关键的升级版本，这可能会让它在人们的堆栈中再停留几年。它的新 LLAP 升级版(不要担心首字母缩略词的含义)主要被认为是一个稳定的遗留选项，允许短时间运行的查询在“交互”时间内返回。以前，无论多小，都很难在不到五秒钟的时间内运行任何查询。

[Impala](https://web.archive.org/web/20230326022526/http://blog.cloudera.com/blog/2016/08/bi-and-sql-analytics-with-apache-impala-incubating-in-cdh-5-8-3x-faster-on-secure-clusters/)(7 月份为 2.6)和[Spark](https://web.archive.org/web/20230326022526/http://spark.apache.org/releases/spark-release-2-0-0.html)(7 月份为 2.0)在大型查询中均有较大的性能提升。Presto 一直在稳步改进，最终在 11 月 30 日发布了 AWS 的 Athena[公告，这是一款管理完善的 Presto S3 产品。](https://web.archive.org/web/20230326022526/https://aws.amazon.com/about-aws/whats-new/2016/11/introducing-amazon-athena-a-pay-as-you-go-interactive-query-service-that-makes-it-easy-to-analyze-data-in-amazon-s3-using-standard-sql/)

> 没有人因为使用云提供商的托管数据仓库而被解雇。

有了这些势头和成熟，像 [Teradata](https://web.archive.org/web/20230326022526/https://www.crunchbase.com/organization/teradata#/entity) 、Vertica 或 Aster 这样的公司越来越难赢得新客户。与 Linux、Apache 或 WordPress 的出现非常相似，它们分别关闭了操作系统、网络服务器和博客软件类别，一个类别中强大的开源赢家既可以关闭该类别，让新的专有进入者进入，也可以让竞争对手注定缓慢衰落。虽然在这方面还没有出现一个单一的赢家，但这一趋势似乎已经非常确定，总体上“Hadoop 上的 SQL”越来越像是大规模分析数据仓库的新默认值。

## 云提供商管理的数据仓库

随着 Azure [宣布其基于 SQL Server](https://web.archive.org/web/20230326022526/https://blogs.technet.microsoft.com/dataplatforminsider/2016/07/12/the-elastic-future-of-data-warehousing/)–的数据仓库于 7 月份全面上市，三大云托管公司(亚马逊、谷歌和微软)都推出了可行的完全托管数据仓库产品。虽然 [对每种技术的相对优点有不同的看法](https://web.archive.org/web/20230326022526/https://aws.amazon.com/blogs/big-data/fact-or-fiction-google-big-query-outperforms-amazon-redshift-as-an-enterprise-data-warehouse/) ，但越来越普遍的做法是，只需点击几下你现有的托管服务提供商，就可以决定使用哪种数据库技术。2016 年很可能是一个新的真理扎根的一年:“没有人因为使用他们的云提供商的托管数据仓库而被解雇。”

在其他新闻中，微软对开源世界日益软化的立场导致了以前无法想象的事情——SQL Server 现在运行在 Linux 上！3 月[高调宣布，11 月](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/03/07/microsoft-is-bringing-sql-server-to-linux/)[全面上市](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/11/16/microsofts-sql-server-for-linux-is-now-available-for-testing/)，这标志着微软通常的以 Windows 服务器为中心的巨大转变——希望是进一步开放的标志。

## 商业智能应用

商业智能应用领域最大的新闻，或者说人们用来从上述数据仓库中提取数据的应用，很大程度上围绕着三大云托管提供商。

微软的产品通常需要三个版本才能完全成熟。2016 年， [Power BI](https://web.archive.org/web/20230326022526/https://techcrunch.com/2015/07/10/microsoft-takes-power-bi-out-of-preview-open-sources-power-bi-visualization-stack/) 从一个有趣的占位产品发布变成了一个相当实用的产品发布。它感觉已经进入了 2.0 阶段，鉴于它的历史，它将获得巨大的动力(和客户)。

> 一旦大公司让你进入他们的流程，他们就不会倾向于做太多的手脚。

房间里的大象刚刚决定醒来，开始伸腿。[亚马逊商务智能产品 QuickSight](https://web.archive.org/web/20230326022526/http://venturebeat.com/2016/11/15/aws-launches-quicksight-business-intelligence-tool-out-of-preview/) 于 2016 年 11 月上市。如果你是一家依赖于成为[红移](https://web.archive.org/web/20230326022526/https://aws.amazon.com/redshift/)的“默认”接口的公司，你可能已经开始失眠了。生态位有被填满的习惯，时间会告诉我们亚马逊是否能够开发出一款面向终端用户的应用。到目前为止，AWS 所有的成功都集中在基础设施上，而不是终端用户界面。然而，Redshift 作为 AWS 上任何人的默认数据仓库的优势越来越明显，加上 AWS 的增长率，使 QuickSight 非常值得一看。数据仓库附近有大量的支出，亚马逊正在协调一致地争夺它。

不想被冷落，谷歌在五月宣布了一个叫做数据工作室的报告和仪表板工具。

## Qlik 私有化了

如果你在美国/硅谷， [Qlik](https://web.archive.org/web/20230326022526/https://www.crunchbase.com/organization/qlik-technologies#/entity) 是你一直忘记的最大的商业智能公司。嗯，托马斯·布拉沃想起来了，于是在六月[](https://web.archive.org/web/20230326022526/http://www.businesswire.com/news/home/20160602005740/en/Qlik-Announces-Agreement-Acquired-Thoma-Bravo-30.50)把他们私了。事实证明，SaaS 公司是绝佳的收购对象，这已成为硅谷最糟糕的秘密。如果你拿一家 SaaS 公司来说，它的产品和采用率都很高，但增长却停滞不前，除去工程、客户支持和会计方面的骨干人员，现金流看起来非常非常诱人。

虽然在一个公司的产品生命周期中过早这样做是有风险的，但是一旦大公司让你进入他们的流程，他们就不会倾向于做太多的改动。所有的“软件”的利润率与 SaaS 增长的现金低谷没有一点关系。有什么不喜欢的？

## Salesforce 浪潮

Salesforce 推出 Wave 时暴露出的一个有趣的可能性是，它将推动公司从 BI 类别中获得可观的收入。这似乎没有奏效。相反，Salesforce 似乎正押注于垂直化，3 月份推出了针对社区云的 [【分析】](https://web.archive.org/web/20230326022526/https://www.salesforce.com/blog/2016/03/introducing-wave-analytics-community-cloud.html) (例如，将分析结果嵌入其他应用程序中) [专用营销分析](https://web.archive.org/web/20230326022526/http://www.pardot.com/blog/salesforce-announces-wave-b2b-marketing-analytics-every-b2b-marketer/) 和 [金融服务](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/09/01/salesforce-wave-catches-vertical-focus-with-new-industry-specific-apps/) 以及 9 月份发布的一般而言 [宣称它是其他人的平台](https://web.archive.org/web/20230326022526/https://techcrunch.com/2015/06/18/new-salesforce-wave-analytics-app-washes-ashore/)

这很大程度上打消了 Salesforce 直接成为 BI 领域主要参与者的可能性，看起来更像是为 force 应用程序添加报告功能的一种方式。

## （舞台上由人扮的）静态画面

Tableau 今年发布了一个新版本，有更多的连接器、数据集群功能、更好的移动使用、跨数据库连接和重新设计。然而，与过去几年相比，增长放缓，亏损增加。这一点，加上 LinkedIn 的声明，导致 Tableau 的股价在 2 月[SaaS 末日](https://web.archive.org/web/20230326022526/http://fortune.com/2016/02/04/tableau-earnings/)下跌了一半，至今仍未恢复。到处都不景气。

## 潜望镜升得很大

加入 Looker 的“是否达到逃逸速度？”俱乐部，[潜望镜](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/11/04/periscope-data-pulls-in-25-million-in-series-b/)在 11 月从贝塞麦筹集了 2500 万美元的 B 轮融资。它非常适合作为一个自带数据仓库(read: Redshift)加上一个托管缓存层。也就是说，随着 QuickSight 的发布，他们和许多其他乘坐“前端红移”浪潮的初创公司处于一个棘手的位置。他们现在直接与 AWS 的产品竞争，尽管这些产品可能还很初级。今年，大多数这类应用程序都迅速增加了对 big query T4 的支持，并希望使他们的客户群多样化。

## 数据收集

将你的交互数据导入 Redshift，使用 BI 应用程序代替 [Mixpanel](https://web.archive.org/web/20230326022526/https://www.crunchbase.com/organization/mixpanel#/entity) 和 friends，开始从前沿走向普遍接受的智慧。

在亚马逊(Amazon)将交互数据纳入红移的几乎但不完全存在的产品(移动分析+数据管道)的影响下，在“将数据纳入红移”细分市场中出现了一些整合。在许多层面上，这些公司的存在实际上更像是对 AWS 的数据移动选项是多么笨重和麻烦的控诉。

> 这出戏的展开是云计算提供商的增长接管了新主机的大部分份额的结果。

随着许多初创公司逐渐沉寂，市场出现了一点震荡。第一批赢家似乎正在浮出水面。细分市场继续拥有当前细分市场+红移+BI 应用程序堆栈的开发人员心智份额。 [Panoply](https://web.archive.org/web/20230326022526/https://techcrunch.com/2016/08/03/panoply-io-raises-7m-series-a-for-its-data-analytics-and-warehousing-platform/) 于 8 月从英特尔投资获得 A 轮融资， [Alooma](https://web.archive.org/web/20230326022526/https://www.crunchbase.com/organization/alooma#/entity) 于 2014 年从红杉获得融资，目前仍在强劲增长。早期的全包式云分析提供商 RJMetrics 于 8 月将其云 BI 产品出售给 Magento，并围绕其数据管道产品成立了一家新公司。

## 整体情况

这场游戏的展开是云计算提供商接管新主机的大部分份额的结果。当你的所有基础设施都在 AWS、Azure 或 Google Compute 上时，你有充分的理由不使用你的提供商的完全托管的数据仓库解决方案。

墙上也写着同样的云提供商将提供这些数据的前端。再加上一些分析师和数据基础设施支出，你就可以在空中获得一个完全统一的数据仓库，其成本只是 10 年前谷歌、脸书或网飞的零头。

大多数垂直分析提供商将需要开始对“为什么我不能在我公司的红移数据上运行你提供的所有 SQL 查询？”双人 SaaS 垂直分析公司的淘金热将开始变得越来越严峻。