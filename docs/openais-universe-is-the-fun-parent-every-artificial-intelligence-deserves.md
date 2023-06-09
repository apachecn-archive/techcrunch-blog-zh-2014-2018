# OpenAI 的宇宙是每个人工智能都值得拥有的有趣父母

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/12/05/openais-universe-is-the-fun-parent-every-artificial-intelligence-deserves/>

# OpenAI 的宇宙是每个人工智能都值得拥有的有趣父母

每个家长最大的噩梦是学生花更多的时间玩电子游戏和上网，而不是为学校学习。但是 OpenAI 的团队相信“有趣的父母”方法实际上可以让我们更接近难以捉摸的广义智能。它的新工具 Universe 是用来训练和测量视频游戏、应用程序和网站的人工智能框架的。

[在一个高层次上，Elon Musk 和 Sam Altman](https://web.archive.org/web/20230326030144/https://techcrunch.com/2015/12/11/non-profit-openai-launches-with-backing-from-elon-musk-and-sam-altman/) 的十亿美元项目 OpenAI 旨在通过民主化来减少人工智能的潜在危害。 [Universe 将推出](https://web.archive.org/web/20230326030144/https://universe.openai.com/) Atari 2600 款游戏、1000 款 flash 游戏和 80 种浏览器环境，目标是加速创造能够擅长多项任务的通用智能。

这个新工具与之前的项目如 ImageNet 一样运行[。ImageNet 数据库是一个巨大的、手工标记的图像集。研究人员多年来一直使用它来测试他们的图像识别系统，并争夺准确性。Universe 更进一步，用 flash 游戏、网络浏览器、照片编辑器甚至 CAD 软件取代了图像。](https://web.archive.org/web/20230326030144/https://en.wikipedia.org/wiki/ImageNet)

《宇宙》让它如此酷的一个特征是它对现实世界的适用性。在这类任务中很容易找到人类表现的基准。玩电脑游戏或浏览网页远没有让一个样本小组在图像中标注树木、汽车和云那么不靠谱。

“4 月，我们推出了 Gym，这是一个用于开发和比较强化学习(RL)算法的工具包，”OpenAI 在一篇博客文章中解释道。"有了 Universe，任何程序都可以变成健身房环境."

强化学习是机器学习的一个分支，它利用奖励的思想来优化问题的解决。强化学习的方法来自行为主义教学，即行为是由明确的奖励和惩罚驱动的。[今年早些时候，DeepMind 发表了一篇关于强化学习在掌握雅达利游戏中的应用的论文](https://web.archive.org/web/20230326030144/http://www.kandroid.org/board/data/board/singularityisnear/file_in_body/1/dqn.pdf)。

当然，要使奖励明确，首先需要创建一个奖励函数，由一些动态值驱动。对于一款 Atari 游戏来说，这相对容易——只是游戏分数。但是为了使这种方法普遍适用，OpenAI 必须建立一个基于卷积神经网络的 OCR 模型。该模型允许通过不断变化的复杂排版和背景图像轻松解析游戏分数。一旦被解析，游戏数据可以直接插入到强化学习奖励函数中。

像网页浏览这样的其他任务不像视频游戏那样清晰，但这并不意味着它们遥不可及。OpenAI 创建了它所谓的“比特的迷你世界”,对简单和复杂的浏览器任务进行基准测试。

如果研究人员能够以一般化的方式在其中一些任务上达到非常高的准确性，人工智能将能够解决 Siri 或谷歌助手等当今平台无法解决的问题。OpenAI 用机票预订的例子来描述未来，人工智能可以操纵网站搜索并最终预订机票。