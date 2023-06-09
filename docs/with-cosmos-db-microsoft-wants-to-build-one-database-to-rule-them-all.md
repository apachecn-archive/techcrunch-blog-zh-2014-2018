# 有了 Cosmos DB，微软想建立一个数据库来统治他们所有人

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/10/with-cosmos-db-microsoft-wants-to-build-one-database-to-rule-them-all/>

“我们希望这个成为未来的数据库，并持续几十年，”微软技术人员 Dharma Shukla 在我们谈论 Cosmos DB 时告诉我，这是该公司今天在其 Build developer conference 上发布的新的全球分布式数据库。对于 Shukla 来说，这是一个始于七年前的项目，当时他开始制作一个全球分布式(或“行星级”，微软经常这样称呼它)数据库的原型。这个项目(当时被称为“佛罗伦萨项目”)最初变成了 DocumentDB，Azure 的 NoSQL 数据库服务，于 2015 年推出，现在正在演变成 Cosmos DB。

用 Shukla 的话说，Cosmos DB 是 DocumentDB 所能提供的“一个重大飞跃”。DocumentDB 只提供了现在的 Cosmos DB 的一部分功能。虽然 DocumentDB 本质上是 JSON 数据的存储，但 Cosmos DB 走得更远。它扩展了无索引数据库系统的概念，并增加了对各种新数据类型的支持，这使得 Cosmos DB 具有足够的灵活性，可以作为图形数据库或键值数据库。对于那些希望存储更传统的列关系数据的人，Cosmos DB 也将提供支持。

【T2![](img/844bce9daed2117179162c28121d95d2.png)

所有这些都是由一句口头禅驱动的，这些天当你与微软开发部门的人交谈时，你几乎不可避免地会听到这句话:“无论开发人员在哪里，我们都希望与他们见面。”因此，虽然您也可以使用 MongoDB APIs 来访问 DocumentDB 中的数据，但 Cosmos DB 也支持 SQL、Gremlin 和 Azure 表——该团队计划在不久的将来推出大量类似的驱动程序和转换层。

“没有数据是天生相关的，”舒克拉告诉我。“在现实世界中，没有人会考虑模式——如果你是 IOT 设备，他们会考虑图形或者 JSON 文档。[……]我们希望确保我们构建的系统有一个通用的引擎来高效地映射不同的数据模型。”

鉴于其传统，Cosmos DB 从 DocumentDB 中获取许多线索也就不足为奇了。其中之一是可调一致性模型的可用性。如果你不花时间考虑全球分布式数据库，那么一致性模型可能对你来说并不那么重要，但大多数竞争数据库系统(包括谷歌最近推出的 [Cloud Spanner](https://web.archive.org/web/20230320033634/https://cloud.google.com/spanner/) )只提供两种一致性模型:强一致性和最终一致性。例如，对于强一致性，每当数据写入数据库时，所有不同的节点(可能分布在全球各地的数据中心)都必须在新值在应用程序中可见之前达成一致。鉴于额外的延迟，这带来了一些明显的性能折衷。最终一致性本质上是一个更宽松的系统，随着时间的推移，所有节点不会同时更新，而是在一段时间内没有任何更新后才会同意某个值。

[![](img/513bf164cf5610d666cf2ebb5049f6eb.png)](https://web.archive.org/web/20230320033634/https://techcrunch.com/wp-content/uploads/2017/05/2017-05-08_1535.png)

“Cosmos DB 的不同寻常之处在于，它提供了不同的一致性模型，用户可以在获得多少一致性和受到多少性能影响之间进行权衡，”莱斯利·兰波特(Leslie Lamport)告诉我，他是[图灵奖得主](https://web.archive.org/web/20230320033634/http://amturing.acm.org/award_winners/lamport_1205376.cfm)，他的工作支撑了许多这些概念(他还编写了 [LaTeX](https://web.archive.org/web/20230320033634/https://en.wikipedia.org/wiki/LaTeX) 文档准备系统)，并于 2001 年加入微软研究院。Cosmos DB 为不同的用例提供了三种不同风格的一致性。“这种中介一致性保证在人们用来写论文的学术系统中已经存在，”Lamport 解释说。Cosmos DB 是首批提供这种一致性模型的商业数据库系统之一。

对于 Cosmos DB(以及以前的 DocumentDB)，这意味着您可以选择一种一致性模型，例如，在这种模型中，读取只允许滞后于写入一定的毫秒数，或者选择一种模型，这种模型侧重于为特定的客户端会话提供一致性(例如，在类似 Twitter 的应用程序中)，但在这种模型中，每个用户在同一时间(甚至以完全相同的顺序)看到每个写入并不那么重要。

[![](img/d3c52f9a14ac68ce6dfde8bd37bf67e8.png)](https://web.archive.org/web/20230320033634/https://techcrunch.com/wp-content/uploads/2017/05/build2017-5100118.jpg)

正如 Shukla 指出的，他的想法是建立一个可以持续几十年的数据库系统。为了做到这一点，他还请来兰波特来教导团队 [TLA+](https://web.archive.org/web/20230320033634/http://lamport.azurewebsites.net/tla/tla.html) 。Lamport 长期以来一直对开发人员如何规范他们的应用程序特别感兴趣。TLA+本质上是一种正式的语言。“当我们在 2010 年开始时，我们想建立一个系统——一个持久的系统。这是微软未来的数据库，”舒克拉告诉我。“我们试图尽可能地将严谨应用到我们的工程中。[……]TLA+在让工程师团队达到这种严谨水平方面表现出色，为质量设立了高标准。”Lamport 指出，TLA+允许你以完全正式的方式进行系统的高层次设计——因为它是正式完成的，所以也可以检查其正确性(公平地说， [AWS 和其他](https://web.archive.org/web/20230320033634/http://lamport.azurewebsites.net/tla/amazon.html)也使用 TLA+来规范他们的分布式系统)。“我不想给人留下 TLA+很棒、我很聪明的印象。它很棒，因为它几乎完全基于数学，”兰波特补充道。

Cosmos DB 对自己的工程能力感觉很强，因此它也提供了许多 SLA，这些 SLA 在数据库领域有些不同寻常。虽然通常保证一定程度的正常运行时间，但微软也为吞吐量、一致性和延迟提供 SLA。“我非常自豪的是——我们觉得这是一份遗产——它是用精心的工艺完成的，”舒克拉说。

值得注意的是，作为微软的传统，Cosmos DB 在微软内部已经使用了很长时间。在其前身 DocumentDB 中，Cosmos DB 目前服务于“成千上万的客户”，微软称，并存储数 Pb 的数据。

Cosmos DB 现已在 34 个 Azure 地区上线，并已全面上市，同时还附带了所有的 SLA 承诺。所有现有的 DocumentDB 客户(及其数据)将自动成为 Cosmos DB 用户。