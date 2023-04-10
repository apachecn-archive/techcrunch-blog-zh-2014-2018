# 谷歌关闭加速网站的 PageSpeed 服务

> 原文：<https://web.archive.org/web/http://techcrunch.com/2015/05/06/google-shuts-down-pagespeed-service-for-accelerating-websites/>

# 谷歌关闭加速网站的 PageSpeed 服务

8 月 3 日，谷歌[将关闭](https://web.archive.org/web/20230316050420/https://developers.google.com/speed/pagespeed/service/Deprecation) [PageSpeed 服务](https://web.archive.org/web/20230316050420/https://developers.google.com/speed/pagespeed/)，这是其托管的优化网站以提高交付速度的解决方案。开发者必须在那之前改变他们的 DNS 设置，否则他们的网站将不再可用。新注册已被禁用。

四年半前推出的 PageSpeed 服务将许多优化技术应用到网站上，以便更快地将其提供给用户。这包括从压缩图像到优化缓存设置、JavaScript 和 CSS 文件。这项服务还缓存静态资产，然后从谷歌在世界各地的服务器上发送出去。在许多方面，PageSpeed 服务类似于 CloudFlare 所做的，但不关注安全性。

![PageSpeed - PageSpeed — Google Developers](img/ae347a365a118342cc6cbe505ce3cb0b.png)因为谷歌还通过开源的 Apache 服务器、NGINX 和其他网络服务器工具的模块提供 PageSpeed 的大部分功能，所以在谷歌自己的托管解决方案关闭后，开发者仍然可以使用它。许多主机提供商也已经在他们的服务器上运行 PageSpeed 模块，谷歌特别调用了 [EdgeCast 的 Edge Optimizer](https://web.archive.org/web/20230316050420/http://www.edgecast.com/services/edge-optimizer/) 作为支持 PageSpeed 的替代 CDN 服务。

那么谷歌为什么要关闭这项服务呢？该公司表示，它已经“遗憾地决定，是时候将他们的努力重新集中到其他地方了，并于 5 月 5 日宣布将拒绝 PageSpeed 服务。”不过，值得注意的是，CloudFlare 无疑已经垄断了这个市场，而且感觉谷歌在过去一两年里并没有在这个领域投入太多努力。