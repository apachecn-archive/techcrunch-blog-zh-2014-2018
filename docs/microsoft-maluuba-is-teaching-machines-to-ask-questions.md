# 微软 Maluuba 正在教机器提问 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/10/microsoft-maluuba-is-teaching-machines-to-ask-questions/>

# 微软 Maluuba 正在教机器提问

众所周知，如今的会话助手还有很多不足之处。我们花了很多时间谈论他们在听我们说话方面有多糟糕，在翻译方面更糟糕。但有一点没有得到足够的重视，那就是我们与 Siri、Cortana 和其他设备的对话是单向的。这些系统不知道如何提问——真正的询问反映了对已知信息和所需信息的细微理解。

微软 Maluuba，微软在 1 月份收购的博士研究团队，[一直在努力探索机器学习和问题生成之间的联系，旨在提供一种智能个人助理，超越当今市场领导者的有限能力。](https://web.archive.org/web/20221006084329/https://beta.techcrunch.com/2017/01/13/microsoft-acquires-maluuba-a-startup-focused-on-general-artificial-intelligence/)[在最近的一篇论文中，](https://web.archive.org/web/20221006084329/https://arxiv.org/pdf/1705.02012.pdf)该团队概述了使用循环网络从大量文本中生成问题的方法。

该团队通过结合监督学习和强化学习，扩展了现有的问题生成器。强化学习利用效用的经济概念来分配“点”,以执行被认为是最佳的行动。该模型是为了最大化这个值而构建的，经过多次迭代，它通过不断调整其策略而得到改进。

[https://web.archive.org/web/20221006084329if_/https://www.youtube.com/embed/UIzcIC5RQN8?feature=oembed](https://web.archive.org/web/20221006084329if_/https://www.youtube.com/embed/UIzcIC5RQN8?feature=oembed)

视频

Maluuba 团队优先考虑准确性和语法。目的是能够用恰当的英语提出问题，并且能够提出能够在原文范围内得到回答的问题。根据机器学习模型回答问题的准确程度来衡量生成问题的质量是一个有趣的命题。

如果模型基于这个故事产生问题，那么询问我们正在讨论的研究是由哪家公司撰写的是合理的。问一个关于团队为什么使用循环网络的一般性问题或者问“团队不使用循环网络？”是不合理的

团队向我解释说，提问的能力提高了回答问题的能力。这是因为问题通常只有一个答案，但也有可能提出多个问题，得到同一个答案。

在实践中，Maluuba 的问题生成器可以通过有意收集新信息，变成一个相当元的系统，用于训练其他机器学习模型。更具体地说，问题生成在教育中也有明显的用途——根据课程材料自动生成问题供学生回答。