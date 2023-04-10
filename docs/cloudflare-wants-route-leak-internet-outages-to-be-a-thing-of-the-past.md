# Cloudflare 希望互联网路由泄露成为过去

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/19/cloudflare-wants-route-leak-internet-outages-to-be-a-thing-of-the-past/>

网络中断经常发生。如果不是有人在街上切断电缆，那就是大规模拒绝服务攻击，用垃圾数据敲打互联网的支柱。

还有一个更常见的原因:路由问题。

互联网路由并不性感。但这是互联网运作的基本部分。路由依赖于边界网关协议(BGP)，该协议管理互联网流量在互联网上的路由方式。BGP 依赖于网络运营商之间的信任，不会发送不正确或恶意的数据。但是错误还是会发生，畸形的数据会形成“路由泄露”，导致互联网流量应该去哪里的混乱，而[会导致](https://web.archive.org/web/20230225041608/https://bgpmon.net/bgp-leak-causing-internet-outages-in-japan-and-beyond/)到[的大规模中断](https://web.archive.org/web/20230225041608/https://www.csoonline.com/article/3138934/security/bgp-errors-are-to-blame-for-monday-s-twitter-outage-not-ddos-attacks.html)。

可以预见的是，坏人会利用过度信任的协议进行“路由劫持”通过重定向未加密的流量，它可以被读取和修改。

现在，Cloudflare 希望通过部署一项新功能来阻止路线泄露和劫持，从而让路由问题成为过去。

Cloudflare 告诉 TechCrunch，向其所有客户免费推出资源公钥基础设施(RPKI)将使重新路由流量变得更加困难——无论是意外还是故意的。

简而言之，RPKI 有助于确保流量通过使用加密签名证书验证为合法和正确的路由到达正确的位置。

Cloudflare 的加密主管 Nick Sullivan 说:“当两个网络相互连接时，比如美国电话电报公司和威瑞森，它们会宣布应该向其发送流量的 IP 地址集。" RPKI 是一个安全框架，确保网络只公布其合法的 IP 地址."

Cloudflare 朝着正确的方向推进之前，美国国家标准与技术研究所(National Institute for Standards and Technology)做出了努力，该研究所上周发布了新标准的第一份草案，其中将 RPKI 作为有助于防止路线泄露和劫持的三个组成部分之一。预计未来几周可能会获得批准。

然而，RPKI 并不完美——它在防止泄露方面比劫持更好，Cloudflare 说，但称其举动是从基于信任转向基于认证的路由的“第一个里程碑”。

沙利文说，推动 RPKI 将保护网络免受欺诈性(或意外地)将流量导向错误的地方，“从而产生一个更安全、更稳定的互联网。”

现在，RPKI 的采用率徘徊在大约 8-9%之间，但是只有不到 1%的网络使用严格的 RPKI 验证。

因为它只有在大量网络运营商部署的情况下才会有效。该公司希望通过展示该技术可以轻松实现且成本高效，来鼓励更广泛地采用该技术。

幸运的话，这可能正是它需要的推动力。