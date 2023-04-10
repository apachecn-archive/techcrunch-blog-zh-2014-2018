# Google Cloud Spanner 更新包括 SLA，承诺每年停机时间少于 5 分钟 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/11/14/google-cloud-spanner-update-include-sla-that-promises-less-than-five-minutes-of-downtime-per-year/>

# Google Cloud Spanner 更新包括 SLA，承诺每年停机时间少于 5 分钟

[Cloud Spanner](https://web.archive.org/web/20221006204415/https://cloud.google.com/spanner/) ，谷歌全球分布式云数据库[今天](https://web.archive.org/web/20221006204415/https://cloudplatform.googleblog.com/2017/11/with-Multi-Region-support-in-Cloud-Spanner-have-your-cake-and-eat-it-too.html)获得更新，包括多区域支持，这意味着数据库可以跨区域复制，以降低延迟，提高性能。它还更新了服务水平协议(SLA ),这应该会让客户满意。

根据 Cloud Spanner 产品经理 Deepti Srivastava 的说法，后者表示 Cloud Spanner 数据库将具有 99.999%(五个九)的可用性，这一停机水平相当于每年不到五分钟。

“我们已经设计了一个高度可用和高效的系统，我们希望服务能够提供这一点，”她说。值得注意的是，在谷歌将 Cloud Spanner 打包为服务之前，它在内部使用它来运行 AdWords 等产品。从谷歌的角度来看，如果 AdWords 宕机，它就不会赚钱，所以它被设计为保持运行。如今，它的许多流行服务都运行在 Cloud Spanner 上。

“谷歌运行的任务关键型应用程序已经过实战测试，”斯利瓦斯塔瓦解释道。

但是该产品缺乏跨多个地区的支持，这意味着您只能在一个位置存放一个云扳手数据库。如今，随着多区域支持的宣布，这种情况发生了变化，这意味着公司可以将数据库放在离用户更近的地方。这将带来响应速度更快、延迟更低的体验。

当谷歌在今年早些时候宣布[云扳手的测试版](https://web.archive.org/web/20221006204415/https://beta.techcrunch.com/2017/02/14/google-launches-cloud-spanner-a-new-globally-distributed-database-service/)时，听起来几乎是不可思议的。它是一个数据库，为开发人员提供了 SQL 数据库的事务一致性和 NoSQL 数据库的可伸缩性。这是一种罕见的组合，像 Evernote 和 Marketo 这样的公司现在都在使用 Cloud Spanner。

该公司声称您只需点击 4 下鼠标即可启动并运行，但实际上，如果您将现有数据库迁移到 Cloud Spanner，情况可能会更复杂。斯利瓦斯塔瓦说，这真的取决于系统的类型。她说，显然，那些开始使用全新应用程序的公司将比那些重新构建现有数据库系统以使用 Cloud Spanner 的公司发展得更快。