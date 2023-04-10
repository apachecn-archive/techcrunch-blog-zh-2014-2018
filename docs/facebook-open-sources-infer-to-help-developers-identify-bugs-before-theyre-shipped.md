# 脸书开源推断帮助开发者在发布前识别 bug 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/06/11/facebook-open-sources-infer-to-help-developers-identify-bugs-before-theyre-shipped/>

# 脸书开源推断帮助开发者在产品发布前识别 bug

脸书今天[宣布](https://web.archive.org/web/20221208175451/https://code.facebook.com/posts/1648953042007882/open-sourcing-facebook-infer-identify-bugs-before-you-ship)开源[推断](https://web.archive.org/web/20221208175451/http://fbinfer.com/)，这是一个静态程序分析器，公司用它在移动代码发货前发现其中的错误。在内部，该公司使用该工具分析 Android 和 iOS 的脸书应用程序、Facebook Messenger、Instagram 和其他应用程序。

脸书表示，Infer 每个月都会通过扫描代码来发现数百个潜在的漏洞，如[空指针访问](https://web.archive.org/web/20221208175451/https://blog.udemy.com/java-null-pointer-exception/)以及资源和内存泄漏——这些问题很容易导致应用程序崩溃。

![fbinfer](img/4be1f0e5fd89902aa391aaa4c45cd399.png)

显然，脸书以其最快的运输速度而闻名。虽然它可以像发布代码一样快速地修复网络漏洞，但对于移动应用程序来说，这根本不是一个选项，因为在大多数情况下，用户必须下载更新才能获得修复。

虽然脸书主要使用 Infer 来查看 Android Java 代码和 iOS Objective-C 项目，但开发人员没有理由不能使用相同的工具来查看任何其他 C 和 Java 代码。事实上，脸书表示，它也在寻求扩大 Infer 的使用范围(或许还有语言)。

在脸书，每当开发人员将代码修改签入该公司一个主要应用的源代码时，Infer 就会自动运行，然后该工具在发现问题时将评论写入代码。

你可以在脸书的博客文章中读到这个工具如何工作的所有技术细节，但值得一提的是，Infer 使用了一个名为“[分离逻辑](https://web.archive.org/web/20221208175451/http://en.wikipedia.org/wiki/Separation_logic)”的概念来发现这些问题。这和有意识的解耦没有任何关系。这种理论允许分析器查看应用存储的一小部分，而不是整个应用。使用它，Infer 可以在 10 分钟内分析大多数代码更改。为了加快速度，Infer 还只查看运行之间发生变化的代码部分。没有这些技术，这种静态分析几乎是不可能的。

推断现在可用[这里](https://web.archive.org/web/20221208175451/http://fbinfer.com/)。