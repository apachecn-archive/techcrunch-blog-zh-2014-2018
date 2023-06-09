# 苹果为 ARM 处理器开源了 iOS 和 macOS 的内核 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/10/01/apple-open-sourced-the-kernel-of-ios-and-macos-for-arm-processors/>

# 苹果为 ARM 处理器开源了 iOS 和 macOS 的内核

苹果一直在每次重大发布后都共享 macOS 的内核。这个内核也可以在 iOS 设备上运行，因为 macOS 和 iOS 都建立在相同的基础上。今年，苹果还在 GitHub 上分享了最新版本的内核[。而且你还可以第一次找到内核的](https://web.archive.org/web/20221127141005/https://github.com/apple/darwin-xnu) [ARM 版本](https://web.archive.org/web/20221127141005/https://opensource.apple.com/source/xnu/xnu-4570.1.46/osfmk/arm64/)。

但首先，是时候了解一些计算机历史了。macOS 的第一个版本(最初命名为 Mac OS X)于 2001 年问世。它建立在由 NeXT 开发的操作系统 [NeXTSTEP](https://web.archive.org/web/20221127141005/https://en.wikipedia.org/wiki/NeXTSTEP) 之上。史蒂夫·乔布斯于 1985 年创建了 NeXT 公司，并于 1997 年将该公司卖回给苹果公司。苹果决定使用 NeXTSTEP 作为 Mac OS X 的基础。

NeXTSTEP 本身就是从开源项目 BSD 衍生出来的。这就是为什么你现在使用的 Mac 电脑严重依赖开源技术。这也是为什么苹果每年只发布很小很小一部分 macOS。你不能编译它，运行你自己版本的 macOS，但是其他内核开发者可能会关心这个内核的源代码。

iOS 呢？2007 年乔布斯[第一次推出](https://web.archive.org/web/20221127141005/https://www.youtube.com/watch?v=wGoM_wVrwng)iPhone 的时候，他说 iPhone 的操作系统是一个 macOS fork。“今天，我们将向您展示一项软件突破。比其他手机至少领先 5 年的软件。我们是怎么做到的呢？嗯，我们从一个强大的基础开始——iPhone 运行 OS X，”乔布斯说。“我们为什么要在移动设备上安装如此复杂的操作系统？因为它有我们需要的一切。”

苹果后来把这个操作系统叫做 iPhone OS，然后是 iOS。这不是一个精确的拷贝，因为 iOS 上没有浮动窗口。但是 iOS 和 macOS 使用相同的基于 Unix 的内核 Darwin 以及许多框架。Apple Watch 和 Apple TV 也运行依赖达尔文的 iOS 版本。

所以你现在可以下载苹果内核的 ARM 优化源代码的事实并不意味着什么。也许苹果想分享 iPhone 的内核，以获得开源社区的反馈。也许这意味着苹果正在开发一个运行在 ARM 芯片上的 macOS 版本。也许这是一场意外。也许苹果只是想看看推特上的反应。