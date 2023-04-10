# Cloudflare 与微软和其他公司合作降低带宽成本 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/26/cloudflare-partners-with-microsoft-google-and-others-to-reduce-bandwidth-costs/>

向带宽联盟问好，这是一个由 Cloudflare 领导的新组织，承诺为许多云客户降低带宽价格。这里的总体想法是，同时使用 Cloudflare(本周将满八岁)和作为该联盟一部分的云提供商的客户将在他们的出口流量上获得显著折扣，或者根本不必为此付费。

该联盟是开放的，其他人仍可能加入，但现在它几乎包括了所有你听说过的主要和次要的云提供商——只有一个例外。目前的成员包括 Automattic、Backblaze、Digital Ocean、DreamHost、IBM Cloud、Linode、Microsoft Azure、Packet、Scaleway 和 Vapor。其中一些现在将通过 Cloudflare 向共同客户提供免费出口流量，而其他一些将通过 Cloudflare 提供高达 75%的总带宽折扣。

这是一个很好的联盟，但正如 Cloudflare 首席执行官兼联合创始人 Matthew Prince 告诉我的那样，一旦第一个成员加入，其余的部分就会很快到位。

但是，为什么这些企业会选择放弃一个小而高利润的业务呢？普林斯说:“我们向他们提出的论点非常简单:当你实际支付运输费时，收取运输费是合理的。”然而，在大多数情况下，这些成本非常小，而 Cloudflare 由于其大量的全球对等位置，可以直接从云提供商那里获取流量，而无需中间人参与。

Cloudflare 是该计划的最初合作伙伴之一，但正如 Prince 所指出的，所有参与方仍有很多需要学习的地方，特别是因为流量有时会以非常不可预测的方式路由，从而绕过成本节约机制。不过，Cloudflare 从中吸取了教训，现在正在使用自己的 [Argo 技术](https://web.archive.org/web/20221025222159/https://www.cloudflare.com/products/argo-smart-routing/)来智能地路由流量。

然而，正如 Prince 指出的，有一件事比预期的要难，那就是确保云供应商知道他们的客户之一是共同客户。有些已经有了这种工具，而 Cloudflare 需要向它们传递一个特殊的头，这样它们就可以知道它们的流量来自哪里。

Prince 还认为，这将使许多公司更容易使用多个云提供商，而不必支付极高的带宽成本。虽然 Cloudflare 的早期重点是 web 流量，但 Prince 表示，现在超过一半的流量是基于 API 的流量，这正是可能因此节省大量资金的用户。

当然，有一家公司没有加入这个联盟，那就是拥有 AWS 平台的亚马逊。普林斯说，Cloudflare 已经和他们谈过了，该组织对所有云和 CDN 提供商开放。

更正:谷歌不是该联盟的成员。