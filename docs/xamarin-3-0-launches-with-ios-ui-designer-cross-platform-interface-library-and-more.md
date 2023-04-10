# Xamarin 3 推出了用于 iOS 应用程序的 UI 设计工具、跨平台界面 API 等 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/05/28/xamarin-3-0-launches-with-ios-ui-designer-cross-platform-interface-library-and-more/>

长久以来，Xamarin 一直是构建[跨平台移动应用](https://web.archive.org/web/20221206232854/https://xamarin.com/tour)最受欢迎的工具之一，今天，[发布了其服务](https://web.archive.org/web/20221206232854/http://blog.xamarin.com/introducing-xamarin-3/)的 3.0 版本，该公司向前迈出了一大步。今天发布的亮点是推出了用于 iOS 的 Xamarin Designer，它几乎可以完全取代用于在 Mac 和 Windows 上设计 iOS 应用的 [Xcode](https://web.archive.org/web/20221206232854/https://developer.apple.com/xcode/) 界面生成器，以及 Xamarin。Forms 是一个为 iOS、Android 和 Windows Phone 应用程序构建共享用户界面代码的 API。

正如 Xamarin 首席执行官兼联合创始人 Nat Friedman 告诉我的那样，这项服务现在已经有超过 60 万名开发人员注册，他认为这是 Xamarin 有史以来最好的版本。

到目前为止，以 C#为中心的 Xamarin 只为 Android 提供用户界面设计器，但在过去两年左右的时间里，该公司也致力于构建 iOS 版本。Designer for iOS 既可以在 Xamarin 自己的 Studio IDE 中运行，也可以在 Visual Studio 中运行。它完全兼容苹果自己的故事板格式，也支持自动布局。

在弗里德曼看来，它在很多方面都比 Xcode 好。他特别指出，Designer 具有更直观的事件处理功能，例如，您总是可以看到自定义控件的实时预览，而不仅仅是最终产品的像素完美表示。然而，最大的吸引力显然是 Xamarin 现在允许 Windows 上的开发人员无需使用 Mac 就可以构建 iOS 应用程序。

鉴于 Android 的 Designer 于 2011 年推出，为什么 Xamarin 花了这么长时间才推出这款产品？弗里德曼认为，他的团队“采取了一种非常雄心勃勃的方法，给你这个像素完美的设计，我们希望确保当我们推出时，你也可以在 Visual Studio 和 Windows 上做到这一点。”

Xamarin。表单也是该公司的一个主要版本。传统上，Xamarin 与其他跨平台开发工具总是有点不同，因为它将应用程序逻辑与接口分离。您可以很容易地在平台之间共享您的应用程序代码，但是您通常会为每个平台开发一个本机接口。不过，正如弗里德曼指出的，Xamarin 的一些客户有大型应用程序，不想在多个平台上为每个屏幕编写新的用户界面。

对于表单，他们得到一个 API，可以访问大约 40 个不同的控件(比如按钮、进度条、滑块等等)。)可以跨平台使用(他们也可以创建自己的控件)。如果你愿意，你也可以很容易地混合搭配使用 Xamarin。表单和本机用户界面。当应用程序被编译时，Xamarin 将呈现本机代码，使用这个 API 抽象层几乎没有性能损失。

你可以使用这些控件构建一个完整的应用程序，但弗里德曼预计，这将特别吸引其平台上的新手开发者和拥有大型移动企业应用程序的公司。

作为今天更新的一部分，该公司还增加了对使用 [F#函数式编程语言](https://web.archive.org/web/20221206232854/http://fsharp.org/)构建 iOS 和 Android 应用程序的支持，以及对。NET 包管理系统 NuGet 和 Visual Studio 13 的共享项目，让跨平台代码共享变得更加容易。Xamarin 现在也支持 Android 4.4 的实验性[艺术运行时](https://web.archive.org/web/20221206232854/https://source.android.com/devices/tech/dalvik/art.html)。

除了所有这些更新之外，Xamarin 今天还宣布收购了 Clarius Consulting 的一个部门，clari us Consulting 是一家总部位于阿根廷布宜诺斯艾利斯的公司，是。网咨询世界。Xamarin 已经收购了负责 Clarius Visual Studio 大部分工作的团队，Friedman 告诉我，该团队现在将全职负责 Xamarin 的产品(Xamarin 本身没有兴趣做任何咨询，Friedman 强调说)。