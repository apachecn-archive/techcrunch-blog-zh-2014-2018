# 微软的 JavaScript 引擎将很快支持 Mozilla 的 ASM . js 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/02/18/microsofts-javascript-engine-will-soon-support-mozillas-asm-js/>

# 微软的 JavaScript 引擎将很快支持 Mozilla 的 Asm.js

在过去的几年里，Mozilla 已经开发了 T2 ASM . js T3，这是一个可以快速执行的 JavaScript 子集。到目前为止，asm.js 优化只在 Firefox 中可用。但是[很快](https://web.archive.org/web/20221207103937/https://blog.mozilla.org/luke/2015/02/18/microsoft-announces-asm-js-optimizations/)这项技术[也将](https://web.archive.org/web/20221207103937/http://blogs.msdn.com/b/ie/archive/2015/02/18/bringing-asm-js-to-the-chakra-javascript-engine-in-windows-10.aspx)在微软即将发布的 Windows 10 的 Chakra JavaScript 引擎中可用。

正如该公司今天宣布的那样，asm.js 支持长期以来一直是开发人员要求最多的十大功能之一，Chakra 团队已经决定实现它。这是对 asm.js 的一次巨大的信任投票，这可能意味着更多的开发人员现在将更仔细地研究这项技术。

“在过去的几个月里，我们仔细研究了 asm.js 作为一项技术、相关技术以及它们对整个网络的影响。尽管手工编写具有挑战性，但 asm.js 主要是通过传输 C/C++代码来在 Web 平台上运行，利用了 WebGL 和 Web Audio 等技术，”Chakra 团队[今天写道](https://web.archive.org/web/20221207103937/http://blogs.msdn.com/b/ie/archive/2015/02/18/bringing-asm-js-to-the-chakra-javascript-engine-in-windows-10.aspx)。“Asm.js 是实现网络平台接近原生性能的一个明显步骤，这就是为什么我们很高兴在即将到来的版本中将其引入 Chakra。”

asm.js 背后的主要思想是，开发人员将他们的 C/C++代码编译成 JavaScript 语言的这个优化子集(使用 [Emscripten 编译器](https://web.archive.org/web/20221207103937/https://github.com/kripken/emscripten))，然后浏览器可以执行。当然，开发人员也可以编写他们自己的 asm.js 兼容代码，但这必然是项目的重点。在当前形式下，asm.js 代码的运行速度比相同的 C/C++代码慢 1.5 倍。

这使得将移动和桌面游戏(原始桌面或移动游戏的代码基础很可能是用 C 编写的)移植到浏览器上变得非常容易。如果没有 asm.js，你可能会在这些游戏中看到相当多的口吃。因为代码仍然是完全标准的 JavaScript，它也可以在任何其他浏览器上运行——只是没有那么快。

![BenchmarkGraph_windows](img/feac5d061417200aaabd78b890031354.png)