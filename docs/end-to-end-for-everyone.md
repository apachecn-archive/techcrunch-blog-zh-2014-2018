# WhatsApp 与 Open WhisperSystems 合作，每天对数十亿条信息进行端到端加密

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/11/18/end-to-end-for-everyone/>

对喜欢隐私和安全的人来说是好消息，对黑帽黑客和政府监控机构来说是坏消息。广受欢迎的消息应用 WhatsApp 已经与加密专家在[Open whispers systems](https://web.archive.org/web/20230406203747/https://whispersystems.org/)合作，对所有 WhatsApp 短信实施[强端到端加密](https://web.archive.org/web/20230406203747/https://whispersystems.org/blog/whatsapp/)——这意味着即使扎克本人也无法窥探你的对话，即使法院命令要求这样做 ¹ 。

当然，WhatsApp 在全球拥有数亿日活用户，今年早些时候被脸书以令人瞠目的 190 亿美元收购。Open WhisperSystems 创建了最先进的端到端加密系统，如用于语音的 [Signal](https://web.archive.org/web/20230406203747/https://techcrunch.com/2014/07/29/talk-private-to-me-free-worldwide-encrypted-voice-calls-with-signal/) ，用于文本的 [TextSecure](https://web.archive.org/web/20230406203747/https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms&hl=en) 。(它们与消息应用 Whisper 无关。)根据 EFF 的[安全信息记分卡](https://web.archive.org/web/20230406203747/https://www.eff.org/secure-messaging-scorecard)，TextSecure 是 WhatsApp 之前加密的[巨大升级](https://web.archive.org/web/20230406203747/https://whispersystems.org/blog/advanced-ratcheting/)。

我指的是巨大的。目前，TextSecure 协议只在 WhatsApp for Android 上推出——其他客户端和群组/媒体消息也即将推出——但引用 OWS 创始人莫邪·马林斯派克的话说，已经“每天有数十亿条加密消息被交换……我们相信这已经代表了历史上最大规模的端到端加密通信部署”。

类似地，这是在苹果加密 iOS 8 设备之后发生的，这样[苹果就无法检索存储在这些设备上的数据](https://web.archive.org/web/20230406203747/http://www.washingtonpost.com/business/technology/2014/09/17/2612af58-3ed2-11e4-b03f-de718edeb92f_story.html)(尽管是以一种封闭的、无法验证的方式。)美国联邦调查局局长詹姆斯·科米[随后声称](https://web.archive.org/web/20230406203747/http://www.nytimes.com/2014/10/17/us/politics/fbi-director-in-policy-speech-calls-dark-devices-hindrance-to-crime-solving.html)“后斯诺登钟摆”已经“走得太远了”，人们担心世界正在“走向黑暗”，走向窃听和监控。由于 WhatsApp 的巨大全球影响力，他们和其他三个字母的机构——以及世界各地的黑帽黑客和政府——不会对他们无法窥探 WhatsApp 短信内容的新能力感到高兴。

然而，科米的说法似乎有一点缺点，那就是不真实:

我认为，对于联邦调查局和国家安全局对越来越多的公司广泛使用端到端加密感到沮丧，以及科技行业“[向他们挑起战争](https://web.archive.org/web/20230406203747/http://www.theguardian.com/technology/2014/nov/04/nsa-cyberwar-stewart-baker-cloudflare-snowden)”的说法，科技行业的回应可以总结为:

公平地说，在一个监视技术似乎每周都在变得更加强大和普遍的世界里，任何对隐私和匿名的有意义的打击都是受欢迎的再平衡。WhatsApp 让这一切成为可能，马林斯派克向他们提出了这个想法，强调他们的热情、奉献和彻底给他留下了深刻的印象，并开放 WhisperSystems 让这一切成为可能。

马林斯派克说，OWS 自己的目标是继续生产强大的开源隐私和安全工具，公司(和个人)可以很容易地将其纳入自己的服务，而不必做自己的密码研究和/或协议设计。他们将继续致力于 Signal 和 TextSecure 作为参考实现，用它们来挑战极限和证明新的想法；与此同时，他们的 TextSecure 协议一下子就拥有了数亿的日常用户，比除了极少数公司之外的所有公司都多。

嗯，算是吧，我的意思是，不完全是。正如一位专家朋友指出的，除了服务器端窃听/中间人攻击之外，还有许多方法可以剥这只特殊的猫的皮；app 后门，设备击键记录者等。