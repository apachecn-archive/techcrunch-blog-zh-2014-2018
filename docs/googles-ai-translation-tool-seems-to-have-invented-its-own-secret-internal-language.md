# 谷歌的 AI 翻译工具似乎发明了自己的秘密内部语言

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/11/22/googles-ai-translation-tool-seems-to-have-invented-its-own-secret-internal-language/>

# 谷歌的 AI 翻译工具似乎发明了自己的秘密内部语言

好吧，不要惊慌，但是*计算机已经创造了它们自己的秘密语言，并且可能正在谈论我们*。嗯，这有点过于简单化了，最后一部分显然是不真实的。但是*有一个*，这是谷歌的人工智能研究人员最近偶然发现的一个迷人且具有生存挑战性的发展。

你可能还记得九月份，谷歌[宣布其神经机器翻译系统已经上线](https://web.archive.org/web/20230321153431/https://techcrunch.com/2016/09/27/google-unleashes-deep-learning-tech-on-language-with-neural-machine-translation/)。它使用深度学习来产生更好、更自然的语言之间的翻译。酷！

继这一成功之后，GNMT 的创造者对一些事情感到好奇。如果你教翻译系统把英语翻译成韩语，反之亦然，也把英语翻译成日语，反之亦然……它能把韩语翻译成日语，而不用英语作为它们之间的桥梁吗？他们制作了这个有用的 gif 来说明他们所谓的“零镜头翻译”的想法(就是橙色的那个):

[![image01](img/401ef8cc96dc925bde261245b6726bad.png)](https://web.archive.org/web/20230321153431/https://techcrunch.com/wp-content/uploads/2016/11/image01.gif)

**图片来源:**谷歌

[事实证明——是的！它在两种语言之间产生“合理的”翻译，而这两种语言并没有以任何方式明确地联系起来。记住，不允许说英语。](https://web.archive.org/web/20230321153431/https://research.googleblog.com/2016/11/zero-shot-translation-with-googles.html)

但这引发了第二个问题。如果计算机能够在没有正式联系的概念和单词之间建立联系……这是否意味着计算机已经为这些单词形成了一个共享意义的概念，其意义在更深的层次上不仅仅是一个单词或短语与另一个单词或短语等价？

换句话说，计算机*是否开发了自己的内部语言*来表示它用来在其他语言之间翻译的概念？基于各种句子在神经网络的存储空间中是如何相互关联的，谷歌的语言和人工智能研究人员认为是这样的。

[![A visualization of the translation system's memory when translating a single sentence in multiple directions.](img/b979be8af670d23692e9839315066b07.png)](https://web.archive.org/web/20230321153431/https://techcrunch.com/wp-content/uploads/2016/11/transcape.png)

从多个方向翻译一个句子时，翻译系统内存的可视化。**图片来源:**谷歌

这种“中间语”似乎是作为一种更深层次的表征而存在的，它看到了所有三种语言中一个句子或单词之间的相似之处。除此之外，很难说，因为复杂神经网络的内部过程难以描述。

它可能是复杂的，也可能是简单的。但是，从哲学的角度来说，它存在的事实——系统自身的原创，以帮助它理解它没有被训练理解的概念——是非常强大的东西。

描述研究人员工作的论文(主要是关于有效的多语言翻译，但也触及了神秘的国际语言)[可以在 Arxiv](https://web.archive.org/web/20230321153431/https://arxiv.org/pdf/1611.04558v1.pdf) 阅读。毫无疑问，系统正在创造和使用的更深层次的概念的问题将需要进一步的研究。在那之前，让我们做最坏的打算。