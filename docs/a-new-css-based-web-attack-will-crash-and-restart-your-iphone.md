# 一种新的基于 CSS 的网络攻击会使你的 iPhone 崩溃并重启

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/09/15/a-new-css-based-web-attack-will-crash-and-restart-your-iphone/>

# 一个新的基于 CSS 的网络攻击将崩溃并重启你的 iPhone

一名安全研究人员发现了一种让任何一部 iPhone 崩溃并重启的新方法——只需要几行代码。

Sabri Haddouche 在[推特上发布了一个概念验证](https://web.archive.org/web/20230307140213/https://twitter.com/pwnsdx/status/1040944750973595649)网页，只有 15 行代码，如果被访问，就会崩溃并重启 iPhone 或 iPad。macOS 上的用户在打开链接时也可能会看到 Safari 死机。

Haddouche 告诉 TechCrunch，该代码利用了 iOS 的网络渲染引擎 WebKit 的一个弱点，苹果要求所有应用程序和浏览器都使用该引擎。他解释说，在 CSS 的背景滤镜属性中嵌套大量元素(如<div>标签)，可以耗尽设备的所有资源并导致内核崩溃，从而关闭并重启操作系统以防止损坏。

“任何在 iOS 上呈现 HTML 的东西都会受到影响，”他说。他警告说，这意味着任何人在脸书或推特上给你发链接，或者你访问的任何网页包含代码，或者任何人给你发电子邮件。

TechCrunch 测试了运行在最新移动软件 iOS 11.4.1 上的漏洞，并确认它崩溃并重启手机。安全公司 Malwarebytes 的 Mac &移动主管托马斯·里德证实，最近的 iOS 12 测试版在点击链接时也死机了。

那些设备不会崩溃的幸运儿可能只会看到他们的设备重启(或“刷新”)用户界面。

对于那些好奇的人来说，你可以[看看它是如何工作的](https://web.archive.org/web/20230307140213/https://gist.github.com/pwnsdx/ce64de2760996a6c432f06d612e33aea)而不用运行导致崩溃的代码。

好消息是，尽管这种攻击令人讨厌，但它不能用于运行恶意代码，他说，这意味着恶意软件不能运行，数据不能通过这种攻击被窃取。但是没有简单的方法来阻止攻击。在邮件中点击一个陷阱链接，或者打开一封显示代码的 HTML 电子邮件，就能让设备立即崩溃。

Haddouche 上周五就攻击事件联系了苹果公司，据称苹果公司正在进行调查。一位发言人没有立即回应置评请求。