# 猎捕机器人的推特机器人嗅出虚假的政治推特 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/10/25/botometer-twitter-bot-hunting-probabot/>

如果你曾经想知道，你将要在 140 个字符中剔除的标签沉重、政治上遥远的 Twitter 用户是否完全是妄想，或者仅仅是不太有感觉，那么，不要再想了。

本周一， [Quartz](https://web.archive.org/web/20221209133454/https://twitter.com/probabot_/status/922590335230009344) 刚刚推出了一款名为@ [的便捷 Twitter 机器人，用于从 Twitter 众所周知的麦田里自动分拣大量谷壳。Probabot 识别政治推文，然后使用一种名为](https://web.archive.org/web/20221209133454/https://twitter.com/probabot_/)[僵尸计](https://web.archive.org/web/20221209133454/https://botometer.iuni.iu.edu/#!/)的东西进行分析，这是由印第安纳大学网络科学研究所和复杂网络与系统研究中心开发的工具。

后一个项目让用户通过机器学习来分析 Twitter 账户，以了解一个账户被自动化的可能性。帐户也可以归入“机器人辅助”类别，这意味着机器人式的自动驾驶和人工干预的结合。

使用 Botometer API，Probabot 在潜在的僵尸轴上扫描帐户，包括他们何时发推文，他们的推文内容在情绪上是积极还是消极，他们在推文中标记了谁，多久一次，以及他们的网络中还有谁。概率创造者基思·柯林斯(Keith Collins)向 TechCrunch 解释了他的机器人如何通过避免经过验证的用户和组织账户等事情来避免误报，这些用户和组织账户有时会表现出一些类似机器人的行为。正如柯林斯解释的那样，被僵尸工具评级超过 48%的账户被标记为潜在的僵尸，而超过 60%的账户被评级为“可能的”僵尸。

Twitter 没有提供太多关于其 bot 问题可能有多普遍的见解，只表示约有 5%的账户是“假冒或垃圾账户”。即使这个数字是一个准确的估计，考虑到这些机器人是如此多产，它们可能会对平台上的政治话语产生巨大的影响。正如 Quartz 所指出的，自 2016 年 4 月以来，Probabot 名单上的一个可能的机器人已经发了超过一百万次推特，这是即使是最忠诚的推特用户也无法实现的。

正如 Botometer 背后的研究人员之一，Emilio Ferrara 博士向 [Quartz](https://web.archive.org/web/20221209133454/https://qz.com/1110481/this-new-twitter-account-hunts-for-bots-that-push-political-opinions/) 解释的那样，“我们发现，在 2016 年大选前一个月活跃在政治对话中的用户中，大约有 15%可能是机器人……他们负责大约五分之一的此类政治推文(近 20%)。”

费拉拉告诉 TechCrunch:“在过去一年左右的时间里，机器人的使用已经从政治宣传转移到在这个国家煽动混乱和分裂。”“通过机器人传播错误信息目前主要涉及围绕社会问题的分裂性信息，对我们社会的影响比以往任何时候都更大。”

概率是一个有用的项目，但值得记住的是，它只能确定某个东西是否可能是机器人。到目前为止，Probabot 已经制作了一份包含 35 个可疑账户的[运行列表](https://web.archive.org/web/20221209133454/https://twitter.com/probabot_/lists/probably-bots/members)，所以随着数据集的扩大，有必要回头看看它们有什么共同点。最终，这些工具与 Botometer 创造者围绕社交平台上的机器人研究的更大研究目标相结合，他们已经[发表了大部分研究成果](https://web.archive.org/web/20221209133454/https://botometer.iuni.iu.edu/#!/publications)。在 2017 年，这是非常值得一读的东西。