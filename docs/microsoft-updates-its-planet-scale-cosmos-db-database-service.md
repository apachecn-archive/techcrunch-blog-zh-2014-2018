# 微软更新其全球规模的宇宙数据库服务 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/24/microsoft-updates-its-planet-scale-cosmos-db-database-service/>

[Cosmos DB](https://web.archive.org/web/20230124090823/https://docs.microsoft.com/en-us/azure/cosmos-db/) 无疑是微软 Azure 组合中最有趣的产品之一。这是一个全面管理的全球分布式多模型数据库，提供吞吐量保证、多种不同的一致性模型和高读写可用性保证。这听起来有点拗口，但基本上，这意味着开发人员可以构建一个真正的全球产品，向 Cosmos DB 写入数据库更新，并确保世界各地的其他用户将在大约 20 毫秒内看到这些更新。例如，为了编写他们的应用程序，他们可以假装 Cosmos DB 是一个与 SQL 或 MongoDB 兼容的数据库。

CosmosDB 于 2017 年 5 月正式推出，尽管在许多方面它是微软现有文档数据库产品的演变，后者远没有那么灵活。今天，微软自己的很多产品都运行在 CosmosDB 上，包括 Azure 门户网站本身，以及 Skype、Office 365 和 Xbox。

今天，微软正在扩展 CosmosDB，推出了多主机复制功能，并支持 Cassandra API，为开发人员提供了另一种选择，将现有产品引入 Cosmos DB，在这种情况下，这些产品是为 Cassandra 编写的。

微软现在也承诺 99.999%的读写可用性。以前，它的读取可用性承诺是 99.99%。虽然这似乎不是一个很大的区别，但它确实表明，在与客户一起运营 Cosmos DB 一年多之后，微软现在更有信心认为它是一个高度稳定的系统。此外，微软还更新了其写延迟 SLA，现在承诺在第 99 百分位小于 10 毫秒。

![](img/a1da3bf499c86784413602b27c057417.png)

微软 CosmosDB 架构师兼产品经理 Rimma Nehme 告诉我:“如果您有跨多个地理区域的写繁重工作负载，并且您需要这种近乎实时的数据接收，这对于物联网、web 和移动游戏场景来说极具吸引力。她还强调，她认为微软的 SLA 定义远比其竞争对手更严格。

不过，此次更新的亮点是多主机复制。“我们相信，我们真的是市场上第一个以如此规模运行的运营数据库，并将为客户提供全球可扩展的多主数据库，”Nehme 说。“底层协议从一开始就被设计成多主协议。”

这有什么大不了的？有了它，开发人员可以将他们运行 Cosmos DB 的每个区域指定为一个独立的主区域，这使得系统在向数据库写入更新方面具有更好的可伸缩性。不需要首先写入可能很远的单个主节点，然后让该节点将更新推送到每个其他区域。相反，应用程序可以写到最近的区域，Cosmos DB 从那里处理一切。如果有冲突，用户可以根据自己的需要决定如何解决。

![](img/298c9bf9ee0c289b034a4c9d709b09bb.png)

Nehme 指出，所有这些仍然可以很好地与 CosmosDB 现有的一套[一致性模型](https://web.archive.org/web/20230124090823/https://en.wikipedia.org/wiki/Consistency_model)一起使用。如果您没有花时间考虑数据库一致性模型，那么这可能听起来很神秘，但是计算机科学的整个领域只关注如何最好地处理两个用户几乎同时尝试更改分布式数据库中的同一个单元格的情况。

与其他数据库不同，Cosmos DB 允许各种一致性模型，从强到最终，有三种中间模型。事实上，大多数 CosmosDB 用户选择了其中一种中间模型。

有趣的是，当我与开发了这些一致性模型(以及流行的 LaTeX 文档准备系统)背后的一些基本概念的图灵奖获得者 Leslie Lamport 交谈时，他并不完全确定开发人员正在做出正确的选择。“我不知道他们是否真的明白后果，也不知道他们的客户是否会感到意外，”他告诉我。“如果他们聪明的话，他们会得到他们所需要的一致性。如果他们不聪明，这意味着他们试图获得一些效率，他们的用户可能会不高兴。”他指出，当你放弃强烈的一致性时，往往很难理解到底发生了什么。

但是强一致性也有它的缺点，这会导致更高的延迟。Lamport 指出:“为了实现强一致性，一定数量的往返消息延迟是不可避免的。

CosmosDB 团队不仅仅建立在 Lamport 围绕数据库所做的一些基础工作之上，而且还广泛使用了 Lamport 在 90 年代末开发的正式规范语言 [TLA+](https://web.archive.org/web/20230124090823/https://lamport.azurewebsites.net/tla/tla.html) 。微软，以及亚马逊和其他公司，现在正在培训他们的工程师使用 TLA+来描述他们的算法，然后再用他们喜欢的语言实现它们。

“因为[cosmos db]是一个非常复杂的系统，没有办法确保它的正确性，因为我们是人，试图将所有这些故障条件和复杂性记在任何一个人——一个工程师——的头上是不可能的，”微软技术负责人达摩·舒克拉指出。“TLA+在使用 TLA+工具正确完成设计、指定和验证方面非常出色，甚至在编写一行代码之前。您涵盖了所有成千上万的边缘情况，这些情况可能会导致数据丢失或可用性损失，或者您从未想过的竞争情况，但在两三年前部署代码后，这些情况可能会导致客户的一些数据损坏。那将是灾难性的。”

“编程语言有一个非常精确的目标，那就是能够编写代码。我一直反复强调的是，编程不仅仅是编码，”Lamport 补充道。“这不仅仅是编码，这是编程中最简单的部分。编程的难点在于正确的算法。”

Lamport 还指出，他故意选择让 TLA+看起来像数学，而不像另一种编程语言。“它真的迫使人们在代码层面之上思考，”Lamport 指出，并补充说，工程师经常告诉他，它改变了他们的思考方式。

至于那些不使用 TLA+或类似方法的公司，兰波特说他很担心。“(微软)使用 TLA+让我感到非常欣慰，因为我看不出任何人在不使用这种数学思维的情况下能够做到这一点——我担心我们最终使用的其他系统是由其他组织构建的——我担心它们有多可靠。”

[https://web.archive.org/web/20230124090823if_/https://www.youtube.com/embed/-4Yp3j_jk8Q?feature=oembed](https://web.archive.org/web/20230124090823if_/https://www.youtube.com/embed/-4Yp3j_jk8Q?feature=oembed)

视频

[![more Microsoft Ignite 2018 coverage](img/b07caa4006a3ed5ee15a0a78966bf3f6.png)](https://web.archive.org/web/20230124090823/https://techcrunch.com/tag/Microsoft-Ignite-2018)