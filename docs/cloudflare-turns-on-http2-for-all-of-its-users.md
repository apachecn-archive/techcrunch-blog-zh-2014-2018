# Cloudflare 为其所有用户打开 HTTP/2 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2015/12/03/cloudflare-turns-on-http2-for-all-of-its-users/>

今年早些时候，[HTTP/2](https://web.archive.org/web/20230129233533/https://en.wikipedia.org/wiki/HTTP/2)——支持网络的 HTTP 协议的继任者——的规格最终确定。但是，正如任何旨在取代互联网如此重要的一部分的技术一样，人们接受它还需要一段时间。然而，HTTP/2 网站的数量今天将会翻倍，因为 [Cloudflare](https://web.archive.org/web/20230129233533/http://cloudflare.com/) 现在默认其所有免费和专业用户都使用[的新协议](https://web.archive.org/web/20230129233533/https://www.cloudflare.com/http2/)(高层客户可以选择使用它)。

正如 CloudFlare 首席执行官 Matthew Prince 告诉我的那样，该公司认为这一举措意味着它现在将为 Alexa 排名前 100 万的网站中 75%的 HTTP/2 部署提供支持。

普林斯说:“互联网的基础协议上一次发生变化是在 1998 年，所以我们很高兴我们在推动支持代表互联网未来的协议方面发挥了重要作用。”

Cloudflare 实际上在上周开始悄悄开启这项服务，这样它就可以毫无问题地让其现在的 400 万客户和 70 个数据中心位置使用新协议。Prince 告诉我:“因为我们可以根据用户类型和地理位置进行细分，所以它允许我们进行部署，这样当它在全球范围内对所有客户可用时，我们就可以确切地知道它将如何执行。”

在很多方面，HTTP/2 都是基于谷歌用 SPDY 做的工作。它允许明显更快的连接，并使大量对象并行传输到浏览器变得更容易，而没有 HTTP/1.x 带来的开销。

顺便说一下，Cloudflare 仍然支持 SPDY。普林斯说，公司决定这样做是因为该团队担心用 HTTP/2 完全取代 SPDY 实际上会使互联网变慢。“一些提供商已经决定淘汰 SPDY，代之以 HTTP/2，”他说。“问题是支持 SPDY 的浏览器仍然比支持 HTTP/2 的浏览器多。”

那么 HTTP/2 比 HTTP/1.x 连接快多少呢？Cloudflare 表示，在其网络上的平均网站上，页面加载时间大约缩短了三秒。不过，Prince 也指出，SPDY 连接和 HTTP/2 连接之间的性能差异并不显著。

尽管有这些优势，CloudFlare 并没有为其业务和企业级客户默认打开 HTTP/2。Prince 告诉我，他建议他们这样做，但就目前而言，Cloudflare 正在为这些用户提供可选服务，这些用户可能希望比公司的大多数用户更好地控制他们的基础架构。不过，从明年的某个时候开始，Cloudflare 也会将这些层中的所有新客户默认为 HTTP/2。