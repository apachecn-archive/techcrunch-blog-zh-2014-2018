# 谷歌让公司更容易将数据传输到它的云 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/03/09/google-makes-it-easier-for-companies-to-transfer-data-to-its-cloud/>

# 谷歌让公司更容易将数据转移到它的云端

今天在谷歌的云下一次会议上，该公司宣布了一系列新工具来帮助用户准备和整合数据。这些更新增强了谷歌企业云的能力和灵活性。

第一个版本是 Google Cloud Dataprep 的新私有测试版。Dataprep 使数据准备过程更加可视化。该工具包括异常检测，并采用机器学习来建议可以提高数据质量的数据转换。

为了使这一过程民主化，谷歌优先考虑界面的整洁，选择通过拖放来实现控制。Dataprep 被优化为与 GCP 集成，这意味着它可以在[谷歌云数据流](https://web.archive.org/web/20221007011216/https://cloud.google.com/dataflow/)中创建管道，以便轻松导出到 [BigQuery](https://web.archive.org/web/20221007011216/https://cloud.google.com/bigquery/) 。

BigQuery 本身也受到了谷歌的关注，推出了新的 BigQuery 数据传输服务。该版本背后的想法是简化合并来自多个来源的数据的过程。这些功能随着对来自 Xignite、HouseCanary、Remind、AccuWeather 和 Dow Jones 的商业数据集的支持而增加。

当连接到 Tableau 等可视化服务时，用户可以无缝地准备和显示分析。BigQuery 现在将支持大型项目的云 Bigtable，因此用户不必浪费时间将数据从一个系统复制到另一个系统。

“我们让营销团队在 GCP 建立营销分析变得非常容易，”谷歌云平台副总裁 Brian Stevens 说。

Python 开发者将会很高兴地得知，Google 正在为其用于云数据流的 Python SDK 提供全面的可用性。这扩大了 Java 之外的社区。

[云数据实验室](https://web.archive.org/web/20221007011216/https://cloud.google.com/datalab/)也即将全面上市。工作流工具将使使用基于 Jupyter 笔记本的环境和标准 SQL 的开发人员更容易执行数据分析。TensorFlow 和 Scikit-learn 正在获得支持，而批处理和流处理现在可以通过 Cloud Dataproc 使用 Cloud Dataflow 或 Apache Spark。与此同时，针对云数据流的 [Stackdriver Monitoring](https://web.archive.org/web/20221007011216/https://cloud.google.com/monitoring/docs/) 正在转向 beta 版，为 GCP 或 AWS 托管的应用提供监控和诊断。

[![](img/c738a94ebd3fab2714e92e3f6dd6aee2.png)](https://web.archive.org/web/20221007011216/https://beta.techcrunch.com/tag/google-next-2017/)