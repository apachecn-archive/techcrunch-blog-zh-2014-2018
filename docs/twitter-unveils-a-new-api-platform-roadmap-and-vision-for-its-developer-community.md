# Twitter 为其开发者社区 TechCrunch 推出了新的 API 平台、路线图和愿景

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/04/06/twitter-unveils-a-new-api-platform-roadmap-and-vision-for-its-developer-community/>

从历史上看，Twitter 与开发者社区的关系一直不稳定。

它曾经鼓励第三方应用，后来

[restricting them](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2012/08/16/twitter-api-client-apps/)

；那就举办开发者大会

[killing them](https://web.archive.org/web/20221205121613/http://www.cio.com/article/3130992/social-networking/is-twitters-dead-developer-conference-another-nail-in-its-coffin.html)

；推出一套开发工具，

[then selling them](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2017/01/18/google-twitter-fabric/)

；尽管如此

[issuing a mea culpa](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2015/10/21/twitter-ceo-dorsey-apologizes-to-developers-says-he-wants-to-reset-relations/)

该公司未能重新赢得许多人的信任。

今天，Twitter 正试图再次重置开发者关系，[发布了 Twitter API 平台的愿景](https://web.archive.org/web/20221205121613/https://blog.twitter.com/2017/building-the-future-of-the-twitter-api-platform),[首次发布了其计划的公共路线图](https://web.archive.org/web/20221205121613/https://trello.com/b/myf7rKwV/twitter-api-platform-roadmap)。

这里的明显目标是让 Twitter 为开发者准备的东西更加透明，包括统一其 API 平台以及为开发者推出新的 API 和端点。

## 简化 API 平台

首先，Twitter 终于充分利用了对 Gnip 的投资。

Gnip 是 Twitter 的长期合作伙伴和社交数据提供商，[于 2014 年被 Twitter 收购](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2014/04/15/twitter-acquires-longtime-partner-and-social-data-analytics-provider-gnip/)。目标是建立 Twitter 的内部大数据分析团队，并与建立在 Twitter 数据和平台之上的大企业建立直接的数据关系。

然而，这次收购将开发人员分成了不同的阶层。大多数开发人员继续使用自 2006 年以来就存在的标准 REST 和实时流 API。与此同时，较大的软件公司可以利用 Gnip 的企业级 API 对 Twitter 数据做更多的事情。

![](img/1cd65115220fc4e12f35734873df46ec.png)

Gnip 的 API 允许开发人员接入“Firehose”(未经过滤的完整推文流及其所有元数据)，并提供比 REST 和流媒体 API 更多的功能。但它们的定价也面向企业用户。这使得刚刚开始扩大规模的开发商无力承担接入费用。

Twitter 表示，它听到了开发者对此的抱怨，并将在今年晚些时候通过将其 REST 和流媒体 API 与 Gnip 相结合来解决这个问题。我们的目标是创建一个集成的 Twitter API 平台，所有开发者——从独立应用程序开发者到大型企业——都可以使用。

Twitter 解释说，API 将被简化，因此开发人员在扩展时不必处理不同的接入点和交付协议。

“这意味着一个从消防水管过滤数据的 API 一个用于搜索 Twitter 档案的 API 一个获取与账户相关的实时活动的 API 包括推文、直接消息、喜欢和关注，”开发人员倡导者安迪·派珀在一篇博文中写道。

![](img/37fae52607d1379b67c4f8247584983d.png)

## 针对数据和 DMs 的分层访问和新 API

除了这种简化，Twitter 将在今年晚些时候引入新的访问层，包括测试新想法的免费访问、自助服务、随着开发者开始扩展而增加功能的付费访问，以及 Twitter 战略合作伙伴的企业访问。

Twitter 表示，它将清楚每个级别的功能和成本，但没有宣布定价。(我们被告知，今年晚些时候会有)。

Twitter 还将推出新的 API，旨在开发商业解决方案——特别是那些可以迎合 Twitter 自身业务领域的 API，Twitter 希望进一步投资于这些领域:客户服务、机器人和品牌参与。

这包括为基于 Twitter 数据构建解决方案的开发者推出 API——比如那些帮助企业了解要构建哪些产品以及如何营销它们，以及更好地了解他们的客户和他们的想法的 API。

除此之外，Twitter 今天还增加了一个[新的账户活动 API](https://web.archive.org/web/20221205121613/https://dev.twitter.com/webhooks/account-activity) 和新的[端点](https://web.archive.org/web/20221205121613/https://dev.twitter.com/rest/direct-messages)，详细的[在这里](https://web.archive.org/web/20221205121613/https://blog.twitter.com/2017/new-apis-to-power-the-future-of-customer-engagement-in-direct-messages)。

这些公司专注于开放 Twitter 的直接信息，允许开发者为希望与客户聊天的企业开发客户服务应用、聊天机器人或其他工具。它们包括支持更新的 Twitter 功能，如直接消息中的[欢迎消息](https://web.archive.org/web/20221205121613/https://blog.twitter.com/2016/speed-up-customer-service-with-quick-replies-welcome-messages-in-direct-messages)和自动[快速回复](https://web.archive.org/web/20221205121613/https://blog.twitter.com/2016/speed-up-customer-service-with-quick-replies-welcome-messages-in-direct-messages)。

![](img/d16436a240df992e335a69d2c84244c3.png)

Twitter 还展示了几个仍处于私下测试阶段的功能，希望得到开发者的反馈——企业可以使用定制简档来覆盖他们的默认头像，以便客户可以看到他们在 DM 上聊天的人类代理人或机器人的照片，以及供企业收集对他们提供的客户服务体验的反馈的“客户反馈卡”。

Twitter 还详细介绍了其新搜索 API 的计划，该 API 提供免费访问 7 天“回顾窗口”，提供比今天更复杂的查询功能和更高保真的数据检索。

## 新的路线图和规则

最后，Twitter 更新了其自动化规则，以指导聊天机器人开发者；宣布了用新的帐户活动 API 替换用户流和站点流的计划；并宣布了一项计划，将几个端点(公共状态/过滤器、状态/样本和搜索/推文)替换为一个简化的 API，在达到速率限制时提供更多访问。

![](img/197f639e92efa7f5ca3c8fa69d0f2720.png)

或许最重要的是，Twitter 首次发布了到 2018 年初的 API 平台路线图。这详细描述了正在进行的工作，计划的时间，以及未来会发生什么。

Twitter 在这方面的投资——精简和统一其 API 平台以允许开发者扩展——意义重大。但尽管发生了这些变化，该公司与开发商之间的麻烦仍可能困扰着它。

Twitter 之前欺骗过[它自己的合作伙伴](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2015/04/11/twitter-cuts-off-datasift-to-step-up-its-own-b2b-big-data-analytics-business/)和[从开发者的脚下拔出地毯](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2012/08/16/twitter-api-client-apps/)，以反映该公司自己不断变化的利益，因为它试图找出它可以从其平台中获取收入的地方。提供其路线图和增加透明度可能有助于缓解一些担忧，但随着 Twitter 自身的[未来](https://web.archive.org/web/20221205121613/https://beta.techcrunch.com/2016/10/14/salesforce-officially-walks-away-from-twitter-acquisition-for-real-this-time/)继续[不确定](https://web.archive.org/web/20221205121613/https://www.recode.net/2016/9/14/12876560/twitter-acquisition-options-google-facebook-apple)，还不清楚有多少开发者会承担责任。