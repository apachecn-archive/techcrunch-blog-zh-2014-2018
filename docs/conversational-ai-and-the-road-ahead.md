# 对话式人工智能和未来之路

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/25/conversational-ai-and-the-road-ahead/>

凯瑟琳·贝利撰稿人

More posts by this contributor

近年来，我们已经看到越来越多的所谓“智能”数字助理被引入各种设备。在最近的 CES 上，[现代](https://web.archive.org/web/20230314143930/https://techcrunch.com/2017/01/03/hyundai-links-up-with-google-assistant-for-car-voice-commands/)和[丰田](https://web.archive.org/web/20230314143930/https://techcrunch.com/2017/01/06/heres-what-its-like-to-drive-with-toyotas-yui-ai-in-car-assistant/)都宣布了新的车载助手。尽管这些应用背后的技术在不断进步，但人们仍然倾向于对他们的能力感到失望——对“智能”的期望没有得到满足。

尽管通过数据驱动的方法在自然语言处理(NLP)方面取得了长足的进步，但是自然语言

*understanding*

仍然难以捉摸。这

[Winograd Schema Challenge](https://web.archive.org/web/20230314143930/https://en.wikipedia.org/wiki/Winograd_Schema_Challenge)

是最近提出的对图灵测试的改进，用于评估一台机器是否可以被判断为“智能的”它以 Terry Winograd 的名字命名，Terry wino grad 是第一个在挑战赛中使用代词歧义消除问题的例子:

市议会议员拒绝给示威者发放许可证，因为他们害怕暴力。”

这里的“他们”指的是什么——议员还是示威者？如果我们不写“害怕”而写“提倡”会怎么样？这改变了我们对“他们”这个词的理解为什么？对我们来说很清楚，议员更可能害怕暴力，而示威者更可能支持暴力。这一信息对于消除代词“他们”的歧义至关重要，但它不在文本本身中，这使得这些问题对人工智能程序来说极其困难。

第一次 Winograd 模式挑战于去年 7 月举行，获胜的算法在挑战中获得了“比随机稍好”的分数。

## 表达与理解

有一种表示语言单词的技术在许多 NLP 任务中被证明非常有用，比如情感分析和机器翻译。这种表示被称为单词嵌入，它们是从数百万个单词用法示例中训练出来的单词的数学表示，以便捕捉意思。这是通过捕捉单词之间的关系来完成的。举一个经典的例子，一组好的表示法可以通过确保各个向量之间存在特定的数学关系(具体来说，国王-男人+女人=王后)来捕捉“国王对男人就像王后对女人”的关系。

这种矢量化表示是谷歌新翻译系统的核心，尽管它们是整个句子的表示，而不仅仅是单词。新系统“将几个主要语言对的翻译错误减少了 55-85%以上”，并且可以执行零镜头翻译:在没有训练数据存在的语言对之间进行翻译。

考虑到所有这些，听到专注于自然语言处理的领先人工智能研究人员柳文欢·埃齐奥尼讽刺道:“当人工智能不能确定句子中的“它”指的是什么时，很难相信它会接管世界。”

那么，AI 可以在它从未被训练过的语言对之间进行充分的翻译，但它不能确定“它”指的是什么？怎么会这样呢？

## 意义只能被间接捕捉到

当听到单词和句子的矢量化表示如何工作时，人们可能会很容易认为它们确实在捕捉意义，因为有一些理解正在发生。但这将是一个错误。这些表述来源于语言使用的例子。我们对语言的使用是由意义驱动的。因此，派生的表示自然反映了那个意思。但是学习这种表达的人工智能系统并不能直接理解实际意义。

对于许多 NLP 任务来说，缺乏对实际意义的理解并不是一个严重的问题。

不理解“它”在句子中指的是什么不会对翻译准确性产生巨大影响——它可能意味着在翻译成法语时使用“il”而不是“elle ”,但这可能不是什么大问题。

然而，当试图创建一个对话式人工智能时，问题出现了:

![pasted-image-0-5](img/4620451c75f6dbf6a138850bf6373768.png)

根据本[教程](https://web.archive.org/web/20230314143930/https://www.ibm.com/watson/developercloud/doc/conversation/tutorial.html)，您可以使用 IBM 的对话服务创建示例机器人的屏幕截图。

理解代词的所指是进行对话的一项非常重要的技能。如上所述，用于训练执行 NLP 任务的 ai 的训练数据不包括用于消除这些单词歧义的必要信息。这些信息来自于对世界的了解。是否有必要在这个世界上实际充当一个具体化的实体，或者只是简单地将大量的“常识知识”编入程序，以收集必要的信息，这仍然是一个悬而未决的问题。也许是介于两者之间的东西。

## 在限制条件下工作

一些非常聪明的人正在研究人工智能中的自然语言理解问题。在今年最大的人工智能会议 NIPS 2016 上，OpenAI 的研究人员展示了

[A Paradigm for Situated and Goal-Driven Language Learning](https://web.archive.org/web/20230314143930/https://arxiv.org/pdf/1610.03585v1.pdf)

。斯坦福大学的研究人员正在研究交互式语言学习，这种方法认识到为了学习意义而与世界互动的重要性。有趣的是，他们的示例系统向 Terry Winograd 的 SHRDLU 系统致敬，这是一个早期的会话系统，它限制自己对由块组成的世界进行陈述和提问。

![pasted-image-0-6](img/5300032bdd7cf26f8e726b4d87c6498e.png)

Terry Winograd 的早期自然语言理解程序 SHRDLU 只限于陈述由积木组成的世界。由 Ksloniewski(自己的作品) [CC BY-SA 4.0](https://web.archive.org/web/20230314143930/https://creativecommons.org/licenses/by-sa/4.0/) ，通过维基共享

对于今天任何想要构建对话式人工智能的人来说，这样的限制仍然是绝对必要的。亚马逊的 Lex 和 IBM 的 conversation 服务都允许开发者指定他们的应用程序应该工作的约束条件。它们定义了应用程序可以执行的一组意图，并将用户可能请求它们的一组可能方式映射到这些意图。

但是，即使没有解决自然语言理解(这可能需要几十年或更长时间)，也有办法增强这种对话式人工智能体验。上图显示，当之前的请求是“关闭挡风玻璃雨刷”时，一个机器人不理解“现在把它们打开”，这表明当一个完全明确的代词不能被理解时是多么令人失望。这绝对可以用今天的技术解决。

对于任何希望使用这种技术来构建或增强应用程序的人来说，理解今天的人工智能和机器学习能力有哪些可能，哪些不可能是关键。如果你对当前能力的说法没有足够的怀疑，你可能会浪费大量的时间和金钱去做一些(还)做不到的事情。另一方面，如果你过于怀疑，你可能会错过部署当今人工智能技术的机会

[incredibly](https://web.archive.org/web/20230314143930/https://research.googleblog.com/2016/11/zero-shot-translation-with-googles.html) [useful](https://web.archive.org/web/20230314143930/https://www.ncbi.nlm.nih.gov/pubmed/15360876)

和

[profitable](https://web.archive.org/web/20230314143930/http://www.forbes.com/forbes/welcome/?toURL=http://www.forbes.com/sites/laurashin/2015/12/09/kensho-the-financial-answer-machine/2/&refURL=&referrer=#197f179160d3) [ways](https://web.archive.org/web/20230314143930/https://medium.com/talla-inc/talla-for-q-a-is-available-on-slack-today-333b11be375e#.h6z45ghqm)

.

![](img/8070d0d965b8701e71a46558e2b101c3.png)