# Google 的 Dart 编程语言即将进入服务器 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/06/29/googles-dart-programming-language-is-coming-to-the-server/>

几天前在其 I/O 开发者大会上，谷歌悄悄宣布，它正在努力将其 [Dart 编程语言](https://web.archive.org/web/20221210031152/https://www.dartlang.org/)引入 App Engine。

该实现将使用该公司最近推出的托管虚拟机和该服务的定制运行时支持。因为自定义运行时支持仍然处于私人测试阶段，然而，Dart 团队还不能向公众发布这一点，但 Google 在 I/O 上向 Dart 开发人员提供了这一点的预览。

大多数开发人员将 Dart 视为 JavaScript 的竞争对手。从很多方面来说，这是公平的，因为它显然是面向类似的用例，而且谷歌提供了一个内置 Dart 虚拟机的 Chrome 浏览器版本。谷歌还为网络开发者提供了 Dart-to-JavaScript 编译器和大量工具。然而，Dart 背后的野心要大得多，因此该团队将其运行时引入 App Engine 和其他服务器也就不足为奇了。

我得以与 Lars Bak 和 Kasper Lund 坐下来，这两个丹麦人一起发明了 Dart (Bak 也开发了谷歌的 V8 JavaScript 引擎)，聊了聊 Dart 的新闻和状态——以及它的未来。

[https://web.archive.org/web/20221210031152if_/https://www.youtube.com/embed/49BH7nxbBmY?feature=oembed](https://web.archive.org/web/20221210031152if_/https://www.youtube.com/embed/49BH7nxbBmY?feature=oembed)

视频

他们指出，Dart 背后的最初想法一直是创建一种通用编程语言。当他们开始这个项目时，他们不只是想创建一些 JavaScript 的变体。这个想法是创建一个动态类型的语言，开发人员可以很容易地学会，这将提高开发人员的生产力。

正因为如此，团队不仅关注语言的可访问性，还关注开发人员使用语言时需要的其他工具。其中包括 Dart 编辑器，Dart 的主要 IDE 和大量扩展该语言的库。此外，该团队最近还推出了内置 Dart 支持的 Android 版 Chrome 浏览器的开发者版本。Lund 还指出，Dart 编辑器附带了许多工具，可以帮助开发人员在运行时监控他们的程序。在 I/O 上，该团队还展示了 Dart 如何与谷歌的聚合物 web 组件项目及其新的材料设计用户界面语言很好地配合。

在 I/O 大会上，谷歌宣布开发人员现在也可以使用 Docker 在其计算引擎基础设施上部署 Dart，但通过很快在 App Engine 上支持它，开发人员可以更容易地访问谷歌的数据存储、云监控服务和缓存服务。

Dart 开发人员长期以来一直要求的另一件事是 Chrome 中内置的 Dart 支持。当我问贝克这个问题时，他给了我一个会心的微笑，并说车队很快会有更多的消息宣布。Chrome 的内置支持显然会给 Dart 带来巨大的推动。虽然 Dart-to-JavaScript 编译器工作得非常好，但 Dart VM 执行代码的速度要快得多。这也会给开发者更大的动力去使用 Dart，因为谷歌不太可能在浏览器中加入 Dart 支持后就取消它。

展望未来，Bak 告诉我，该团队也在研究如何将异步代码引入类似于 JavaScript 的 [asyn/await](https://web.archive.org/web/20221210031152/http://bjouhier.wordpress.com/2013/06/01/bringing-asyncawait-to-life-in-javascript/) 的概念。

自从该团队推出了 [Dart 1.0](https://web.archive.org/web/20221210031152/http://news.dartlang.org/2013/11/dart-10-stable-sdk-for-structured-web.html) ，它还致力于为 Dart 创建一个 [Ecma 标准(就像 JavaScript 基于 EcmaScript 标准一样)。正如 Bak 所说，没有一种好的编程语言是由 committee 创造出来的，所以对 Google 来说，在开始这个过程之前让 Dart 达到 1.0 里程碑是很重要的。然而，现在它也想让其他行业参与者参与进来，该团队希望其他浏览器能够集成它。](https://web.archive.org/web/20221210031152/http://news.dartlang.org/2013/12/ecma-forms-tc52-for-dart-standardization.html)

Dart 团队认为，能够用同一种语言编写前端和后端代码将使代码更加稳定，并使开发团队更容易合作。