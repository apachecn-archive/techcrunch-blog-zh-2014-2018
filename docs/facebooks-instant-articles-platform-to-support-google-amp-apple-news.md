# 脸书的即时文章平台支持谷歌和苹果新闻

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/25/facebooks-instant-articles-platform-to-support-google-amp-apple-news/>

如今，出版商在使其内容在移动设备上更具可读性时面临的一个问题是，有多种相互竞争的格式可用于此目的。脸书有[即时文章](https://web.archive.org/web/20230316161016/https://instantarticles.fb.com/)，谷歌是 [AMP](https://web.archive.org/web/20230316161016/https://www.ampproject.org/) (加速移动页面)项目的先锋，[苹果新闻格式](https://web.archive.org/web/20230316161016/https://developer.apple.com/news-publisher/)为 iOS 设备优化内容。脸书今天开始尝试解决这个问题，推出了对 AMP 和即将推出的苹果新闻的支持，作为其开源即时文章软件开发包的一部分。

更新后的 SDK 现在将包括一个[扩展](https://web.archive.org/web/20230316161016/https://github.com/facebook/facebook-instant-articles-sdk-extensions-in-php)，允许出版商构建可以以所有三种格式发布的内容，除了脸书自己的即时文章之外，还支持谷歌的 AMP。未来几周，它还将支持发布到苹果新闻，但该公司没有提供该功能将于何时添加的确切发布日期。

在高层次上，SDK 将采用用于构建脸书即时文章的标记，并使用它来创建 AMP 和 Apple News 所需的代码。当然，虽然多个系统并不完全相同，但脸书表示，它将为出版商提供为竞争服务应用定制样式模板的方法，包括应用定制字体、颜色和标题等内容，这些内容将尽可能地反映在其他格式中。

这一改变的目标是提供一次设计，随处发布的体验——从正确的角度来看，发布到脸书自然是第一要务。

该功能将通过对 Facebook Instant Articles SDK 的扩展来实现，该扩展可在 Github 上找到。(关于其用法的文档在脸书开发者网站上，[这里](https://web.archive.org/web/20230316161016/https://developers.facebook.com/docs/instant-articles/other-formats)。)

扩展的想法是作为[脸书新闻项目](https://web.archive.org/web/20230316161016/https://media.fb.com/2017/01/11/facebook-journalism-project/)的一部分产生的，该项目旨在将脸书与媒体出版商联系起来[以帮助通知该公司在其网站](https://web.archive.org/web/20230316161016/https://techcrunch.com/2017/01/11/facebook-journalism-project/)上即将推出的新闻特写的路线图。该项目的其他想法包括让出版商通过脸书免费试用他们的付费订阅，出版商开发团队的黑客马拉松，脸书用户可以订阅的摘要包，在脸书推广新闻素养的公益广告，记者教程等等。

然而，该扩展的推出也正值许多知名出版商开始放弃脸书的格式，因为它缺乏货币化选择。

例如，在四月，据报道，福布斯、赫斯特、纽约时报和其他媒体已经退出了即时新闻。包括彭博、华尔街日报、ESPN、哥伦比亚广播公司新闻、NPR、金融时报和 VICE News [在内的其他主要媒体机构也一直拒不合作，很少甚至没有脸书格式的内容。其他使用这种形式的人已经逐渐减少了他们的支持；上个月,《卫报》退出了脸书的即时文章和苹果新闻。](https://web.archive.org/web/20230316161016/https://digiday.com/media/bloomberg-wsj-others-remain-facebook-instant-articles-holdouts/)

出版商普遍对平台削减收入分成的交易感到不满，也不喜欢即时文章格式阻止他们与读者建立更直接的关系。对于那些不必处理弹出窗口和其他杂乱信息的读者来说，将访问者发送到精简的、移动优化的页面可能是一种很好的体验，但从历史上看，这意味着出版商不能提供与网络上相同的广告，也不能鼓励捐款，推动付费订阅，推广他们的电子邮件简讯或活动，或与读者建立其他联系。

脸书试图通过调整即时文章的规则来消除这些担忧，比如,[允许他们展示更多广告](https://web.archive.org/web/20230316161016/https://techcrunch.com/2017/03/09/deal-with-the-blue-devil/)，或者[推出新功能](https://web.archive.org/web/20230316161016/https://media.fb.com/2017/04/07/launching-call-to-action-units-for-instant-articles/#more-6020)，比如文章中的行动号召单元，可以促进电子邮件注册或请求页面点赞。它让出版商[推出免费试用和应用下载、](https://web.archive.org/web/20230316161016/https://www.bloomberg.com/news/articles/2017-04-07/facebook-adds-signup-buttons-to-win-over-skeptical-news-partners)以及其他服务。

现在，通过将 Facebook Instant 文章与 AMP 和 Apple News 捆绑在一起，该公司希望能够通过使同时发布到所有三大服务成为可能，吸引出版商回到其平台。但是，如果不完全放松限制，如果即时文章的格式不符合出版商的更大目标，脸书可能仍然很难证明这一点。