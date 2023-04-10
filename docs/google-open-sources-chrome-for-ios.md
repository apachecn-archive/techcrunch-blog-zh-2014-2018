# 谷歌开源 iOS 版 Chrome 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/01/31/google-open-sources-chrome-for-ios/>

# 谷歌开源 iOS 版 Chrome 浏览器

谷歌今天[宣布](https://web.archive.org/web/20221206184815/https://blog.chromium.org/2017/01/open-sourcing-chrome-on-ios.html)iOS 版 Chrome 的代码现在是其 Chrome[开源项目](https://web.archive.org/web/20221206184815/https://chromium.googlesource.com/chromium/src.git/+/master/ios/)的一部分。

在 iOS 上，Chrome 不得不使用苹果的 WebKit 渲染引擎，而不是谷歌自己的 Blink 引擎。正因为如此，谷歌之前并没有将 Chrome for iOS 代码添加到 Chromium 代码库中。毕竟，在同一个代码库中支持两种渲染引擎会增加相当多的复杂性。

然而，在过去的几年里，谷歌的团队致力于进行必要的代码修改，将 Chrome for iOS 代码添加到 Chrome 中。这项工作现在已经完成，想要[编译 Chromium iOS 版本](https://web.archive.org/web/20221206184815/https://chromium.googlesource.com/chromium/src/+/master/docs/ios_build_instructions.md)的开发人员现在可以从 Chromium 库获取 iOS 代码并这样做了(当然，假设他们运行 OS X 并使用 Xcode)。

谷歌认为，这一举措也意味着 iOS 版 Chrome 的开发速度将会更快，因为该团队在 Chrome 上运行的所有测试现在也可以自动在 iOS 版 Chrome 代码基础上运行。