# 在 Lyft、Care.com、goPanache TechCrunch 进行早期部署后，Stripe 向所有承包商提供即时支付

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/09/19/stripe-offers-instant-payouts-to-all-contractors-after-early-rollouts-at-lyft-care-com-gopanache/>

与 PayPal 的 Braintree 和 WePay 等为数字企业提供支付服务的初创公司竞争的 Stripe 正在揭开其最新产品的面纱，以使其与众不同。Stripe 正在推出[即时支付](https://web.archive.org/web/20221206140055/https://stripe.com/blog/instant-payouts-for-marketplaces)，这是一项专门为市场定制的服务，可以在“几分钟内”将款项支付给承包商现有的 Visa 或 MasterCard 借记卡。

Stripe 实际上已经为一些客户提供了(并测试了)即时支付的有限服务:乘车服务 [Lyft](https://web.archive.org/web/20221206140055/http://lyft.com/) 、助手市场[Care.com](https://web.archive.org/web/20221206140055/http://care.com/)和理发服务 [goPanache](https://web.archive.org/web/20221206140055/http://gopanache.com/) ，这帮助他们为员工提供了更好的服务，同时相对于其他竞争对手的市场更具竞争力。(Lyft 于去年 10 月推出了这项服务，实际上它上周宣称，到目前为止，它已经通过该计划向司机支付了约 5 亿美元。)

现在，Stripe 正在为任何已经使用 Stripe 的 Connect basic payments API 的市场(首先从美国开始)开放即时支付产品。与 Connect 一样，要使用即时支付选项，公司需要添加几行代码。与 Connect 的情况一样，Stripe 在交易完成时赚钱——在这种情况下，Stripe 收取支付金额的 1.5%，最低费用为 50 美分。

即时赔付解决了一个常见的痛点。像 Lyft、Postmates 和 Airbnb 这样的双边市场是当今科技界发展最快的初创公司之一，因其快速、按需服务模式而广受欢迎。这些市场价值数十亿美元，为消费者提供乘车和外卖等服务，同时也是人们签约提供这些服务的平台。

但这些公司通常不擅长的一件事是按需付费。承包商可能需要几天时间才能从他们提供的服务中获得回报，这也是 Stripe 希望解决的难题。

“只要我们授权交易，资金就有保障,”Stripe 的卡基础设施负责人拉奇·格鲁姆(与 Stripe 的联合创始人约翰·科利森长得一模一样，仅供参考)说。他解释说，之所以会出现这种情况，是因为如今的大多数支付服务(包括 Stripe 的基本 Connect 产品)都使用自动清算网络(T4)来转账，而凭借 Stripe 与 Visa 和 MasterCard 的交易，新服务使用“快速支付”铁路。

Stripe 并不是唯一一家旨在加快客户赔付速度的公司。今年早些时候，优步推出了一个名为“与 GoBank 即时支付”的项目，最初要求承包商使用 GoBank 借记卡收款，但后来“T8”扩大了“T9”覆盖所有基于借记卡的银行账户。

贝宝的 Braintree 也提供 [Venmo Payouts](https://web.archive.org/web/20221206140055/https://www.braintreepayments.com/blog/introducing-a-new-way-to-pay-service-providers-venmo-payouts/) ，尽管据我所知这项服务需要一天的时间才能让资金到达您的账户。

但是对于许多在这些平台上工作以赚取一点外快的承包商来说，或者作为他们的主要收入来源，像 Stripe 的即时支付这样的事情会让他们更快地获得他们所赚的钱，当你考虑到这一点的时候，应该在一个基于实时即时交付的模型中给出。

对于 Stripe 来说，当它在 2015 年最后一次融资时，估值约为 50 亿美元，新服务是与战略投资者 Visa 合作的结果，并表明该公司如何继续多元化其基本支付之外的业务以提高利润率。其他扩展包括帮助外国公司在美国注册的 [Atlas](https://web.archive.org/web/20221206140055/https://beta.techcrunch.com/2016/02/24/stripe-expands-startup-tools-with-atlas-a-way-for-global-companies-to-incorporate-in-delaware/) ，以及它的另一个 [Stripe Connect](https://web.archive.org/web/20221206140055/https://beta.techcrunch.com/2015/03/23/stripes-new-product-helps-marketplaces-go-global-more-quickly/) 产品，专门针对新国家的市场。