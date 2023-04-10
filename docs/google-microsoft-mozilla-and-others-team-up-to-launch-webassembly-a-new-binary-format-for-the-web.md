# 谷歌、微软、Mozilla 和其他公司联手推出 WebAssembly，一种新的 Web  二进制格式

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/06/17/google-microsoft-mozilla-and-others-team-up-to-launch-webassembly-a-new-binary-format-for-the-web/>

[谷歌](https://web.archive.org/web/20230404073509/https://twitter.com/jfbastien/status/611201861245399041)、[微软](https://web.archive.org/web/20230404073509/http://blogs.msdn.com/b/mikeholman/archive/2015/06/17/working-on-the-future-of-compile-to-web-applications.aspx)、 [Mozilla](https://web.archive.org/web/20230404073509/https://blog.mozilla.org/luke/2015/06/17/webassembly/) 和 [WebKit 项目](https://web.archive.org/web/20230404073509/https://bugs.webkit.org/show_bug.cgi?id=146064)的工程师们今天宣布，他们已经合作推出了 [WebAssembly](https://web.archive.org/web/20230404073509/https://github.com/WebAssembly) ，一种新的[二进制格式](https://web.archive.org/web/20230404073509/https://github.com/WebAssembly/design/blob/master/BinaryEncoding.md)，用于编译网络应用。

网络因标准而繁荣，无论好坏，JavaScript 是它的编程语言。然而，这些年来，我们已经看到越来越多的努力，允许开发人员通过构建将其他语言的代码转换成 JavaScript 的编译器来解决 JavaScript 的一些限制。其中一些项目专注于向语言添加新功能(如微软的 [TypeScript](https://web.archive.org/web/20230404073509/http://www.typescriptlang.org/) )或加速 JavaScript(如 Mozilla 的 [asm.js](https://web.archive.org/web/20230404073509/http://asmjs.org/) 项目)。现在，许多这样的项目开始以 WebAssmbly 的形式聚集在一起。

这种新格式旨在允许程序员为浏览器编译他们的代码(目前的重点是 C/C++，其他语言也会跟上)，然后在 JavaScript 引擎中执行。不过，WebAssembly 可以显著加快解码速度，而不必解析整个代码，这通常需要很长时间(尤其是在移动设备上)

这个想法是 WebAssembly 将为开发者提供一个单一的 web 编译目标，最终将成为在所有浏览器中实现的 web 标准。

默认情况下，JavaScript 文件是从服务器下载的简单文本文件，然后由浏览器中的 JavaScript 引擎进行解析和编译。例如，WebAssembly 团队决定采用二进制格式，因为该代码甚至可以比标准 JavaScript 文本文件压缩得更多，还因为引擎解码二进制格式比解析 asm.js 代码快得多(在当前原型中快 23 倍)。

Mozilla 的 asm.js 一直致力于为网络带来近乎本土的速度。谷歌的用于在浏览器中运行本地代码的 [Native Client](https://web.archive.org/web/20230404073509/https://code.google.com/p/nativeclient/) 项目也有类似的目标，但相对来说没什么吸引力。看起来 WebAssemly 现在可以将这些项目中的精华带到浏览器中了。

作为第一步，WebAssembly 团队的目标是提供与 asm.js 大致相同的功能(开发人员将能够为 WebAssembly 使用与他们今天编译 asm.js 代码相同的 Emscripten 工具)。

在这个早期阶段，该团队还计划推出一个所谓的 [polyfill 库](https://web.archive.org/web/20230404073509/https://remysharp.com/2010/10/08/what-is-a-polyfill)，它将把 WebAssembly 代码翻译成 JavaScript，以便它可以在任何浏览器中运行——甚至是那些没有本机 WebAssembly 支持的浏览器(这显然有点荒谬，但一旦浏览器可以本机运行这些代码，就不需要最后一步了)。随着时间的推移，团队将构建[更多的工具](https://web.archive.org/web/20230404073509/https://github.com/WebAssembly/design/blob/master/Tooling.md)(编译器、调试器等)。)并增加对更多语言的支持(比如 Rust、Go 和 C#)。

正如 JavaScript 发明者(和[短期](https://web.archive.org/web/20230404073509/https://blog.mozilla.org/blog/2014/04/05/faq-on-ceo-resignation/) Mozilla CEO) Brendan Eich [今天所指出的](https://web.archive.org/web/20230404073509/https://brendaneich.com/2015/06/from-asm-js-to-webassembly/)，一旦主流浏览器原生支持新格式，JavaScript 和 WebAssembly 将会再次分离。

该团队指出，顺便说一句，这里的想法并不是要取代 JavaScript，而是允许更多的语言为网络编译。事实上，JavaScript 和 WebAssembly 可能会同时使用，应用程序的某些部分可能会使用 WebAssembly 模块(动画、可视化、压缩等)。)，而用户界面仍然主要是用 JavaScript 编写的。

我们很少看到所有主要的浏览器供应商在这样的项目上合作，所以这绝对是未来几个月和几年值得关注的事情。