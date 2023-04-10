# Commons 条款阻止开源滥用

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/07/commons-clause-stops-open-source-abuse/>

Salil desh pande撰稿人

Salil Deshpande 是

[Bain Capital Ventures.](https://web.archive.org/web/20230317103535/http://www.baincapital.com/)

他专注于基础设施软件和开源。

More posts by this contributor

地平线上有一片乌云。亚马逊等云基础设施提供商的行为威胁着开源的生存能力。

在 13 年的风险投资生涯中，我投资了许多开源项目背后的公司:

开源服务于社会，开源商业模式是成功且有利可图的。生活很美好。

## 亚马逊的行为

我很佩服亚马逊的执行力。在风险业务中，我们习惯于大型软件公司(如 IBM、Oracle、HP、Compuware、CA、EMC、VMware、Citrix 等)主要是大型销售和分销渠道，它们需要获得创新(即创业公司)来支持其渠道。不是亚马逊。2015 年 7 月，华尔街日报[引用我](https://web.archive.org/web/20230317103535/https://www.wsj.com/articles/DJFVW00120150708eb78fl2ce)的话说，“亚马逊执行得太好了，几乎就像一家初创公司。这对生态系统中的每个人来说都很可怕。”那个月，我在投资者网站 Seeking Alpha 上写了[恐惧亚马逊巨头](https://web.archive.org/web/20230317103535/https://seekingalpha.com/article/3333195-fear-the-amazon-juggernaut)。自从我写了那篇文章后，AMZN 已经上涨了 400%。(我间接拥有 AMZN。)

但是对于除了顾客之外的任何人来说，亚马逊并不是一个温暖而模糊的公司。[繁](https://web.archive.org/web/20230317103535/https://www.businessinsider.com/what-its-like-to-work-at-amazon-2018-2) [篇](https://web.archive.org/web/20230317103535/https://www.businessinsider.com/here-are-the-14-rules-behind-amazons-brutal-workplace-2015-8) [有](https://web.archive.org/web/20230317103535/https://www.nytimes.com/2015/08/16/technology/inside-amazon-wrestling-big-ideas-in-a-bruising-workplace.html) [详](https://web.archive.org/web/20230317103535/https://www.businessinsider.com/the-worst-parts-about-working-at-amazon-according-to-employees-2015-8/#your-offer-comes-with-a-lot-of-stock-but-it-wont-vest-for-two-years-1)其青黄不接，割喉文化。为什么它对开源的使用会有所不同呢？

转到[亚马逊网络服务](https://web.archive.org/web/20230317103535/https://medium.com/r/?url=https%3A%2F%2Faws.amazon.com) (AWS)并将鼠标悬停在顶部的产品菜单上。你会看到许多开源项目，这些项目不是亚马逊创建的，而是作为服务运行的。这些每年为亚马逊提供数十亿美元的收入。

例如，亚马逊将[Redis](https://web.archive.org/web/20230317103535/https://redis.io/)(stack overflow 的开发者调查中[最受欢迎的数据库](https://web.archive.org/web/20230317103535/https://redislabs.com/press/redis-named-loved-database-second-consecutive-year/))作为一项服务来运行，重新命名为 AWS Elasticache。许多其他流行的开源项目，包括 Elasticsearch、Kafka、Postgres、MySQL、Docker、Hadoop、Spark 等，也同样被作为 AWS 产品提供。

需要明确的是，这并不违法。但是我们认为这是错误的，并且不利于可持续的开源社区。

## 公地条款

2018 年初，我召集了 24 家大规模开源公司的创始人、首席执行官或首席法律顾问，讨论该怎么办，其中一些公司是上市公司。今年三月[,我和 GeekWire](https://web.archive.org/web/20230317103535/https://www.geekwire.com/2018/might-time-big-cloud-share-wealth-open-source-startups/) 谈到了这项工作。经过大量建设性的讨论后，该小组决定，与其拐弯抹角地混合和匹配开源许可证来阻止这种行为，我们应该创建一个直接的条款来禁止这种行为。我们聘请了受人尊敬的开源律师[希瑟·米克](https://web.archive.org/web/20230317103535/https://heathermeeker.com/2018/06/24/revisiting-the-open-source-business-model/)来起草这一条款。

2018 年 8 月，Redis 实验室宣布他们决定将这个被称为[公共条款](https://web.archive.org/web/20230317103535/https://commonsclause.com/)的附加条款(即一个额外的段落)添加到他们针对某些附加模块的自由开源许可证中。Redis 本身将继续使用[许可的 BSD 许可](https://web.archive.org/web/20230317103535/https://redislabs.com/blog/redis-license-bsd-will-remain-bsd/)——Redis 本身没有任何变化！但 Redis Labs 附加模块将包括 Commons Clause rider，它使源代码可用，但不能“出售”模块，其中“出售”包括将它们作为商业服务提供。目标是明确防止云基础设施提供商的不良行为。

任何其他人，包括通用汽车或通用电气这样的企业，仍然可以做他们过去能够用软件做的所有事情，即使应用了公共条款。他们可以查看和修改源代码，并提交 pull-request 以将他们的修改添加到产品中。他们甚至可以在内部为员工提供软件即服务。公地条款阻止的是以云基础设施提供商的方式用别人的开源软件运行商业服务。

不出所料，了解开源社区后，这一声明引起了热烈的反响，有赞成的，也有批评的。冒着过于简单化的风险: [中的](https://web.archive.org/web/20230317103535/https://www.tfir.io/no-redis-didnt-become-proprietary/)[那些](https://web.archive.org/web/20230317103535/https://twitter.com/solomonstre/status/1032390658445594625)[favo<wbr>r](https://web.archive.org/web/20230317103535/https://www.influxdata.com/blog/its-time-for-the-open-source-community-to-get-real/)[视](https://web.archive.org/web/20230317103535/https://blog.tidelift.com/redis-this-is-not-the-license-change-you-are-looking-for-) [这个](https://web.archive.org/web/20230317103535/http://antirez.com/news/120)为[逻辑](https://web.archive.org/web/20230317103535/https://www.i-programmer.info/news/136-open-source/12093-the-commons-clause-.html) [和](https://web.archive.org/web/20230317103535/https://www-zdnet-com.cdn.ampproject.org/c/s/www.zdnet.com/google-amp/article/storj-labs-forges-open-source-vendors-and-cloud-services-alliance/) [积极](https://web.archive.org/web/20230317103535/https://medium.com/@michaeldehaan/why-open-source-needs-new-licenses-d2d9d819a10) [进化<wbr> n](https://web.archive.org/web/20230317103535/https://blog.dgraph.io/post/relicensing-dgraph/) 在开源许可中，允许开源公司在投资开源项目的同时运营可行的业务。[迈克尔·德汉](https://web.archive.org/web/20230317103535/https://medium.com/@michaeldehaan/why-open-source-needs-new-licenses-d2d9d819a10)， [Ansible](https://web.archive.org/web/20230317103535/https://github.com/ansible) 的创造者，在[为什么开源需要新的许可](https://web.archive.org/web/20230317103535/https://medium.com/@michaeldehaan/why-open-source-needs-new-licenses-d2d9d819a10)中，有一部分说得特别好:

> 我们看到有人运行开源“基金会”和网站，这些网站本质上是空谈，对“开源”的定义进行政治辩论，正如所谓的“开源倡议”所描述的那样，它包含各种各样的名称，这些名称已经获得了某种程度的流行或追随者。他们试图声明，这种源代码可以免费获得，但用例有限的许可证“不是开源的”。不幸的是，那艘船已经起航了。

[那些](https://web.archive.org/web/20230317103535/https://drewdevault.com/2018/08/22/Commons-clause-will-destroy-open-source.html) [中立](https://web.archive.org/web/20230317103535/https://drewdevault.com/2018/08/22/Commons-clause-will-destroy-open-source.html) [或](https://web.archive.org/web/20230317103535/https://drewdevault.com/2018/08/22/Commons-clause-will-destroy-open-source.html) [反对](https://web.archive.org/web/20230317103535/https://www.theregister.co.uk/2018/08/23/redis_database_license_change/) <wbr>的人指出，公地条款让软件不开源，这是准确的，让部分代码库专有有违开源的风气；Redis 实验室肯定很绝望，也很难赚钱。

首先，不要担心 Redis 实验室。公司做得非常非常好。而且 Redis 比以往任何时候都更强大，更受喜爱，更 [BSD](https://web.archive.org/web/20230317103535/https://redislabs.com/blog/redis-license-bsd-will-remain-bsd/) 。

更重要的是，我们认为是时候在今天的环境中重新审视开源的精神了。当开源变得流行时，它是为从业者设计的，让他们在对社区做出贡献的同时进行实验和构建。没有一家公司提供基础架构即服务。没有一家公司会接受一个开源项目，重新命名它，将它作为一项服务来运行，保留利润，并且回报很少。

我们的观点是，开源软件从来就不是为云基础设施公司准备的。这并不是开源的初衷。公地条款正在复兴开源的原始精神。学者、业余爱好者或开发人员希望使用一个流行的开源项目来驱动他们应用程序的一个组件，他们仍然可以这样做。但是，如果你想获得别人已经开发的基本相同的软件，并把它作为一项服务来提供，为了你自己的利益，这不符合开源社区的精神。

正如在公共条款的情况下，这可以使源代码在技术上不是开源的。但这是我们必须忍受的，以保持原有的精神气质。

## Apache + Commons 子句

Redis 实验室发布了某些附加模块作为 Apache + Commons 子句。Redis 实验室非常清楚地表明，Commons 条款的应用使它们不是开源的，而且 [Redis 本身仍然是开源的，并且是 BSD 许可的](https://web.archive.org/web/20230317103535/https://redislabs.com/community/licenses/)。

一些狂热的开源专家指责 Redis 实验室试图欺骗社区，让他们认为模块是开源的，因为他们使用了“Apache”这个词。(据报道，他们在提出这些指控时口吐白沫，但公平地说，这可能只是流口水。)

没有诡计。公共条款是附加在任何许可性开源许可证上的附加条款。因为各种开源项目使用各种开源许可证，当发布使用公共条款的软件时，一个必须指定哪个底层许可开源许可证附加了公共条款。

## 为什么不是 AGPL？

在这个场景中，不使用 [AGPL](https://web.archive.org/web/20230317103535/https://www.gnu.org/licenses/agpl-3.0.en.html) 有两个主要原因，一个是开源许可，它规定当你运行 AGPL 许可的代码作为服务时，你必须向公众发布你所做的任何修改。

首先，AGPL 使其变得不方便，但并没有阻止云基础设施提供商参与上述滥用行为。它只是说，他们必须发布他们在从事这种行为时所做的任何修改。第二，AGPL 包含了一些不必要的软件专利的语言，很多企业都不喜欢。

我们投资组合中的许多拥有 AGPL 项目的公司都收到了来自大型企业的请求，要求使用更宽松的许可证，因为使用 AGPL 违反了他们公司的政策。

## 平衡

云基础设施提供商不是坏人，也不是心怀不轨的人。开源一直是一种平衡行为。我们中的许多人相信我们的客户和同行会看到我们的源代码，做出改进并分享回来。免费分发一个人的工作成果，并相信你能够把食物放在桌子上，这总是一种信仰的飞跃。有时候，对于一些项目，不需要太多刻意的努力就能达到自然的平衡。但在其他时候，自然平衡不会出现:我们越来越多地看到基础架构开源，特别是当云基础架构提供商试图通过将堆栈从商用计算和存储移动到更高级别的基础架构服务来实现差异化时。

## 修订

撰写本文时，Commons 子句的版本是 1.0。将来会有修改和调整，以确保公地条款实现其目标。我们希望您能提供[意见](https://web.archive.org/web/20230317103535/https://github.com/fossas/commons-clause)。

到目前为止，我们所看到的关于公地条款的意见分歧实质上是哲学上的分歧。许多批评来自开源的书呆子，他们不从事用软件赚钱的生意。他们有不同的哲学，但这并不奇怪，因为他们的工作是成为政治活动家，而不是在公司中创造价值。

一些人误解为它阻止人们提供维护、支持或专业服务。这是对语言的误读。一些人声称这与 AGPL 教相冲突。Commons 条款旨在与比 AGPL 更宽松的开源许可证一起使用，这样就不必使用 AGPL 了！尽管如此，即使是在 AGPL 案中，很少有作者作品的使用者会认为简单地无视作者意图应用公地条款的声明是谨慎的。

## 保护开源

一些开源利益相关者很困惑。他们应该站在哪一边？公地条款是新的，我们预计会有争论。这项倡议背后的人是坚定的开源倡导者，我们的目的是保护开源免受生存威胁。我们希望其他人也能加入到这项事业中来，这样开源公司就能赚钱，开源也能生存，开源开发者也能因他们的贡献而获得报酬。