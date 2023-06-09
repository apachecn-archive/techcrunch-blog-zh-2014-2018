# 继 AWS 之后，谷歌计算引擎也转向了按秒计费

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/09/26/following-aws-google-compute-engine-also-moves-to-per-second-billing/>

一周前，AWS [宣布](https://web.archive.org/web/20230222071129/https://techcrunch.com/2017/09/18/aws-announces-per-second-billing-for-ec2-instances/)将很快转向对其 EC2 服务的用户按秒计费。因此，谷歌今天[宣布](https://web.archive.org/web/20230222071129/https://cloudplatform.googleblog.com/2017/09/extending-per-second-billing-in-google.html)一个非常相似的举措并不令人惊讶。

Google Compute Engine、Container Engine、Cloud Dataproc 和 App Engine 的灵活环境虚拟机(VMs)现在将提供[每秒计费](https://web.archive.org/web/20230222071129/https://cloud.google.com/compute/pricing)，立即开始(AWS 用户仍需等到 10 月 2 日)。这种新的定价方案扩展到运行高级操作系统的可抢占机器和虚拟机，包括 Windows Server、Red Hat Enterprise Linux 和 SUSE Enterprise Linux Server。因此，它超越了 AWS，后者只为基本 Linux 实例提供每秒计费，而不为 Windows Server 和其平台上的其他 Linux 发行版提供，后者目前提供单独的每小时收费。

和 AWS 一样，谷歌会收取最少一分钟的费用。

值得注意的是，谷歌已经为其持久磁盘、GPU 和承诺使用折扣提供了每秒计费功能。

虽然谷歌辩称，在大多数用例中，每秒计费只会导致非常小的计费变化，但该公司也指出，在许多应用中，能够快速扩大和缩小规模非常有意义(例如，网站、移动应用和数据处理工作)。

“这可能是为什么我们没有听到很多客户要求每秒，”计算引擎集团产品经理 Paul Nash 在今天的公告中写道。“但是，我们不想让您在早上喝咖啡和核心时间之间做出选择，所以我们很高兴为您的虚拟机提供每秒计费，最少一分钟。”

因此，虽然谷歌没有站出来说出来，但这显然是对亚马逊此举的反应，尽管该公司大多将其视为两种云计算服务之间功能比较的另一个复选框。

### 那么微软呢？

到目前为止，微软还没有做出类似的举动。“通过 Azure Container 实例，我们实际上引领了按秒计费的方式，一项服务在几秒内启动，几秒内停止，我们意识到为客户提供这种粒度的成本非常重要，”微软 Azure Compute 产品负责人科里·桑德斯(Corey Sanders)在微软 Ignite 大会上告诉我，当时我问他公司的计划。“我很高兴看到其他云纷纷效仿，为客户提供最大的定价灵活性。”

至于普通的虚拟机，Sanders 坚持认为微软想要专注于容器，因为在那里每秒计费是最有意义的。“我们一直在寻求改进我们整个平台的计费结构，让我们的客户使用起来更容易、更灵活，”他说。不过，如果微软在不久的将来不采取行动也选中每秒计费复选框，我会感到非常惊讶。