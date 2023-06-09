# WhatsApp、Signal 和危险无知的新闻业 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/01/22/whatsapp-signal-and-dangerously-ignorant-journalism/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

关于加密的某些东西会暴露出记者最糟糕的一面。因为对他们中的大多数人来说，这是一种魔力，他们总是不顾一切地寻找谚语中的幕后之人，却不知道要寻找什么。这或许可以解释《卫报》最近对 WhatsApp 的奇怪攻击，他们错误地指责 WhatsApp 有“后门”安全部门勃然大怒。

要理解这个故事，为什么《卫报》是错的，为什么他们被迫退回[他们最初的“后门”标题](https://web.archive.org/web/20230127142347/https://gizmodo.com/theres-no-security-backdoor-in-whatsapp-despite-report-1791158247)，为什么安全社区如此愤怒，你需要一点背景知识。坐下，我的宝贝们，让我告诉你一个小小的信息安全寓言:

从前有 PGP，代表相当好的隐私，它又好又强。如此优秀和强大，以至于在它的创造者菲尔·齐默曼于 25 年前发布了它的源代码后，美国政府以武器走私为由对[展开了刑事调查。(该案后来被撤销，没有起诉。)](https://web.archive.org/web/20230127142347/https://en.wikipedia.org/wiki/Phil_Zimmermann#PGP)

二十年来，PGP 一直是安全消息传递的黄金标准。国家安全局无法破解。爱德华·斯诺登用过。但是它有严重的缺陷。首先，它缺乏前向保密性。如果你的密钥泄露了，那么它加密过的所有信息都会泄露。另一方面，密钥交换过去和现在都很有挑战性。

但到目前为止，PGP 最糟糕的一点是它对用户极其不友好，所以只有铁杆黑客才会真正使用它。(斯诺登的爆料被推迟了一个月，因为他无法找到安全联系格伦·格林沃尔德的方法。)

正如最好的锻炼程序不是岩石的 T1，而是你将真正坚持的，最安全的信息系统是你将真正使用的。不管我们喜欢与否，*可用性是安全性的一个重要方面。任何假装这不是真的“安全”系统都将被废弃不用。*

进入[信号](https://web.archive.org/web/20230127142347/https://whispersystems.org/)，一个移动(和 Chrome 插件)安全消息系统。它快速、灵活、性感、跨平台，并且经过了实战考验。它使用“棘轮”协议实现了高度安全的端到端消息传递，该协议提供了完美的前向保密性。这是全世界技术成熟、安全意识强的人们的选择。它并不完美。没有一个系统是完美的。每个系统都需要妥协。但是信号是最好的选择。

然而，世界上大部分地区并不使用信号。世界上大多数人使用短信、Facebook Messenger，尤其是 WhatsApp——直到最近，WhatsApp 还远不安全。因此，两年前[开始的 WhatsApp 信号协议的推出受到了欢迎。然而，尽管它使用相同的*协议*作为信号，但是*实现*是不同的。《卫报》奇怪而错误地称这种差异为“后门”](https://web.archive.org/web/20230127142347/https://techcrunch.com/2014/11/18/end-to-end-for-everyone/)

有关令人讨厌的细节，请参见 EFF 的“[Whatsapp 中的交易被称为后门](https://web.archive.org/web/20230127142347/https://www.eff.org/deeplinks/2017/01/google-launches-key-transparency-while-tradeoff-whatsapp-called-backdoor)”；Signal 头头莫邪·马林斯派克的“[没有 Whatsapp 后门](https://web.archive.org/web/20230127142347/https://whispersystems.org/blog/there-is-no-whatsapp-backdoor/)”；布鲁斯·施奈尔的“ [WhatsApp 安全漏洞](https://web.archive.org/web/20230127142347/https://www.schneier.com/blog/archives/2017/01/whatsapp_securi.html)”；以及弗雷德里克·雅各布斯的“[关于‘Whatsapp 后门、交易和机会主义认证](https://web.archive.org/web/20230127142347/https://www.fredericjacobs.com/blog/2017/01/20/whatsapp-backdoor/)”。编辑:之前的一个链接被替换了，因为大家一致认为它对 Wire(一个完全不同的私人信息应用)的描述不公平/不准确。)

最重要的问题是，当你与之交谈的人得到一部新手机，或者重新安装了应用程序时，没有办法立即确定新安装的是他们。理论上，你应该通过不同的媒介与他们交流，以验证他们不是伪装成他们的其他人；在一个完美的世界里，你可以使用 Signal 和 WhatsApp 提供的工具来确定这一点。然而实际上，基本上没有人这样做。

Signal 是为技术成熟的用户设计的，它拒绝向一个身份似乎已经改变的人发送任何新消息，除非你明确告诉它这样做。WhatsApp 拥有大约 10 亿用户，其中绝大多数人在技术上并不成熟，当它推出信号协议时，它认为这样做会让用户困惑并导致对话丢失，并且继续传递信息比让用户明确确保他们的安全更重要。

他们这样做是否正确，这是一个理性的人可以不同意的事情。同样，*所有的*消息传递系统都涉及到安全问题；有时候，所有的信息系统都要求你信任某人。当我住在英国时,《卫报》是我选择的报纸，我自己也为他们撰稿，但认为一些人不同意的复杂妥协是“后门”或深刻的隐藏漏洞是非常不负责任的新闻。

一方面，WhatsApp 对 Signal 协议的实现不如 Signal 的实现安全。另一方面,*比他们以前的系统安全得多——唯一能够利用这个漏洞攻击 WhatsApp 信息的实体是 WhatsApp 本身，或者是危及 WhatsApp 系统的入侵者。此外，正如 Schneier [指出的](https://web.archive.org/web/20230127142347/https://www.schneier.com/blog/archives/2017/01/whatsapp_securi.html)，“这是对当前和未来信息的攻击，而不是让政府回到过去的事情。从这个角度来看，这并不比政府窃听你的手机、读取你在 WhatsApp 上的对话更麻烦。”*

更重要的是，WhatsApp 的用户已经不得不信任 WhatsApp。所有他们实际上，可核实地知道，应用程序根本没有实现信号协议。他们还必须信任苹果、谷歌或任何下载应用程序的人。他们必须相信，他们的手机上没有恶意软件正在注册他们的按键和偷拍截图。他们必须相信操作系统[提供了加密算法需要的熵](https://web.archive.org/web/20230127142347/https://github.com/WhisperSystems/Signal-iOS/blob/c7ee430790898110f575adbda5bf34000b32242f/Signal/src/crypto/CryptoTools.m#L13)。你必须永远相信*某人*。这是必然的。即使你从头开始编译 PGP，你也不能一行一行地检查它的代码来确定它是安全的——即使你这样做了，内核又如何呢？[编译器](https://web.archive.org/web/20230127142347/http://wiki.c2.com/?TheKenThompsonHack)怎么样？

真正的安全设计是在可用性和安全性之间找到平衡点，确定用户的复杂程度和威胁模型，决定谁是你必须信任的，谁是你不能信任的。 [Signal 也做出妥协](https://web.archive.org/web/20230127142347/http://arstechnica.com/information-technology/2016/12/signal-does-not-replace-pgp/)——尤其是它对你电话号码的使用。安全设计是一项复杂而模糊的任务，无知的 gotcha 记者无法区分有争议的妥协和“后门”，这不会使安全设计变得更容易。

这不是一个深奥的理论问题:这伤害并危及所有真实的人。说“切换到信号”忽略了一个事实，即大多数人的联系人不会这样做，所以如果他们需要沟通，他们事实上的选择是在 WhatsApp 和 SMS 之间——如果你吓走了前者，你会吓得他们投入后者极其脆弱的怀抱。《卫报》的那些对这一丑陋的混乱局面负有责任的人要对此负责。你不需要相信我的话，但是你应该相信[这个安全世界的名人录](https://web.archive.org/web/20230127142347/http://technosociology.org/?page_id=1687)的话。