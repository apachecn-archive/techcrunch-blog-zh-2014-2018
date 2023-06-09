# Netlify 希望让 web 开发者更容易使用 AWS Lambda 事件触发器

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/03/20/netlify-wants-to-make-it-easier-for-web-developers-to-use-aws-lambda-event-triggers/>

Netlify 的愿景是改变我们开发网站的方式，让前端设计与后端服务执行的连接变得更简单。今天，该公司宣布在 Netlify 上推出 [AWS Lambda 函数](https://web.archive.org/web/20230324211935/https://techcrunch.com/2014/11/13/amazon-launches-lambda-an-event-driven-compute-service/)，这是该愿景的又一步。

该公司旨在降低与网络开发相关的复杂性。你用 HTML 和 JavaScript 设计你的前端，然后 Netlify 帮助你连接到一组你可能正在使用的服务，比如用于支付的 Stripe 或用于电子邮件简讯管理的 MailChimp。Netlify 已经抽象出了网络服务器的概念，称其部署缓慢，难以保护和扩展。通过从单一网站转向具有后端微服务的静态前端，它相信它可以解决安全和扩展问题，并更快地交付网站。

他们不在乎你用什么工具来建设网站。您只需简单地设计它，Netlify 就可以在它执行的边缘直接处理所有后端编码。从这个意义上说，它是内容交付网络一部分，也是开发者自动化引擎一部分。

这种建立更快更动态网站的能力引起了安德森·霍洛维茨公司的彼得·莱文的注意，他在去年 8 月领导了该公司 1200 万美元的首轮投资。“[创始人]有一个绝妙的主意，利用微服务和 API 来构建更灵活、更动态的网站；部署到边缘以创建更高性能的最终用户体验；并与 Github 集成，轻松创建和管理应用程序，”Levine 说。

今天的发布将这种服务方式向前推进了一步。 [Lambda 是 AWS 所谓的无服务器工具](https://web.archive.org/web/20230324211935/https://techcrunch.com/2015/11/24/aws-lamda-makes-serverless-applications-a-reality/)。它使开发人员能够创建基于特定触发事件运行的功能，而不必担心服务器的 24/7 运行。这非常符合 Netlify 的 web 开发方法，它从本质上把 web 服务器从 web 发布过程中移除了。

在这种情况下，该公司创造了一种更简单的方法来运行 Lambda 函数。他们认为，虽然 web 开发人员喜欢事件触发器的想法，但 AWS 工作流太复杂了。通过提供一种更简单的方式来创建事件触发器，尤其是围绕开发者身份，它将降低准入门槛。

“我们看到[Lambda]的前景是显而易见的，但没有围绕它的工作流程这一事实使得它很难使用。我们有前端出版的工作流程，所以[我们决定]让我们对无服务器做同样的事情，”公司联合创始人克里斯蒂安·巴赫解释说。

“每个 Lambda 触发器都变成了一个微小的微服务，你可以通过浏览器与之对话，”他说。例如，要使用 Stripe 进行支付，您需要对您的秘密 Stripe 凭证进行编码，以进入支付网关。“要打这个小电话，你需要从某个地方运行一个服务器。人们会为了那一点点功能而构建一个 Rails 应用程序，”Bach 说。

使用 Netlify 方法，您可以通过几行代码输入您的凭证，然后使用带有一点 Netlify 粘合代码的 Lambda 触发器。他说，这解决了代码存在于何处以及如何管理它的问题。

Levine 认为边缘计算是技术向前发展的一大驱动力，他领导了 Andreessen Horowitz 的首轮投资，并加入了 Netlify 董事会，这可能不是巧合。

“我谈论边缘计算已经有一段时间了，网络生活是更广泛的边缘服务趋势的一部分。该公司已经开发了建立和部署现代网站的方法，”莱文说。

该公司成立于 2015 年，已融资 1410 万美元。