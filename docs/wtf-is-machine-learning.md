# WTF 是机器学习？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/10/23/wtf-is-machine-learning/>

虽然关于机器学习的标题数量可能会让人认为我们刚刚发现了一些非常新的东西，但事实是这项技术几乎和计算一样古老。

艾伦·图灵，有史以来最有影响力的计算机科学家之一，[以“机器能思考吗？”这个问题开始了他 1950 年关于计算的论文](https://web.archive.org/web/20230130011456/http://www.loebner.net/Prizef/TuringArticle.html)，这并非巧合从我们的科幻小说到我们的研究实验室，我们长期以来一直质疑创造人造版本的自己是否会以某种方式帮助我们揭示我们自己意识的起源，以及更广泛地说，我们在地球上的作用。不幸的是，人工智能的学习曲线真的非常陡峭。通过追溯一点历史，我们应该有希望能够弄清机器学习到底是什么。

## 如果我的大数据足够大，我能创造智能吗？

我们复制自己的第一次尝试包括干扰充满信息的机器，并期待最好的结果。说真的，曾经有一段时间，主流的意识理论认为，意识可以从一大堆连接在一起的信息中产生。谷歌可能被一些人视为这一愿景的顶点，但尽管该公司已经索引了 30 万亿个网页，我认为没有人会希望我们的搜索引擎开始问我们是否存在上帝。

相反，机器学习的美妙之处在于，我们不是假装计算机是人类，只是简单地向它们灌输知识，而是帮助计算机进行推理，然后让它们将自己学到的知识推广到新的信息中。

虽然没有得到很好的理解，但神经网络、深度学习和强化学习都是机器学习。它们都是创建能够对新数据进行分析的通用系统的方法。换句话说，机器学习是许多人工智能技术中的一种，像神经网络和深度学习这样的东西只是可以用来建立更好的框架和更广泛的应用的工具。

回到 50 年代，我们的计算能力有限，我们无法访问大数据，我们的算法也很初级。这意味着我们推进机器学习研究的能力非常有限。然而，这并没有阻止人们去尝试。

早在 1952 年，亚瑟·塞缪尔用一种非常基本的人工智能形式——阿尔法贝塔剪枝——制作了一个国际象棋程序。这是一种在使用表示数据的搜索树时减少计算量的方法，但它并不总是解决所有问题的最佳策略。甚至神经网络也在去年用弗兰克·罗森布拉特的感知机露了脸。

## 一个复杂的声音模型，你应该阅读一下

感知器远远领先于它的时代，利用神经科学来推进机器学习。理论上，这个想法看起来有点像右边的草图。

为了理解它在做什么，你首先必须理解大多数机器学习问题可以分解为分类或回归。分类器用于对数据进行分类，而回归模型主要用于推断趋势以进行预测。

[感知器是分类器](https://web.archive.org/web/20230130011456/https://appliedgo.net/perceptron/)的一个例子——它获取一组数据并将其分成多组。在这种情况下，具有各自权重的两个特征的存在足以使该对象被分类在“绿色”类别中。今天，分类器从您的收件箱中分离垃圾邮件，并为您的银行检测欺诈。

Rosenblatt 的模型使用一系列输入，考虑长度、重量、颜色等特征，并给它们分配一个权重。然后，该模型不断调整权重，直到达到落入可接受的误差范围内的输出。

例如，可以输入一个恰好是苹果的物体的重量是 100 克。计算机不知道它是一个苹果，但感知器可以通过调整分类器相对于已知训练数据集的权重，将该对象分类为类似苹果的对象或非类似苹果的对象。一旦对分类器进行了调优，理想情况下，它可以在以前从未接触过的数据集上重用，以对未知对象进行分类。

## 还好，连人工智能研究者都被这东西搞糊涂了

感知器只是机器学习中许多早期进步的一个例子。神经网络有点像一起工作的大量感知机，很像我们的大脑和神经元的工作方式，这就是这个名字的来源。

几十年来，人工智能的进步一直是复制大脑的工作方式，而不是简单地复制我们所感知的内容。基本的或“浅层”的神经网络今天仍在使用，但深度学习已经成为下一件大事。深度学习模型是有更多层的神经网络。对于这个令人难以置信的令人不满意的解释，一个完全合理的反应是问我所说的层是什么意思。

为了理解这一点，我们必须记住，仅仅因为我们说计算机可以将猫和人类组织成两个不同的群体，计算机本身并不以人类的方式处理任务。机器学习框架利用抽象的思想来完成任务。

对人类来说，脸有眼睛。对计算机来说，人脸有明暗像素，这些像素构成了一些抽象的线条。深度学习模型的每一层都让计算机识别同一对象的另一个抽象级别。像素到线条到 2D 到 3D 几何图形。

## 尽管极其愚蠢，计算机已经通过了图灵测试

人类和计算机评估世界的方式的这种根本差异对创造真正的人工智能提出了严峻的挑战。图灵测试的概念是评估我们在人工智能方面的进展，但它在很大程度上忽略了这一现实。图灵测试是一种行为主义测试，专注于评估计算机模拟人类输出的能力。

然而，模仿和概率推理充其量只是智力和意识之谜的一部分。一些人认为我们在 2014 年成功通过了图灵测试，当时一台机器在五分钟的键盘对话中说服了 30 名科学家中的 10 名，认为它是人类(然而 Siri 仍然试图在谷歌上搜索我们问她的每三件事)。

## 那么，我应该得到我的人工智能冬季夹克吗？

尽管取得了进展，但科学家和企业家都很快过度承诺了人工智能的能力。由此产生的繁荣和萧条周期通常被称为 AI winters。

我们已经能够利用机器学习做一些令人难以置信的事情，比如为自动驾驶汽车对视频片段中的对象进行分类，以及利用卫星图像预测作物产量。长短期记忆正在帮助我们的机器处理时间序列，比如视频中的情感分析。强化学习，从博弈论中汲取思想，包括一个通过奖励来辅助学习的机制。强化学习是 Alpha Go 能够击败 Lee Sodol 的关键部分。

也就是说，尽管取得了所有进展，但机器学习的最大秘密是，尽管我们通常知道给定问题的输入和输出，以及作为中介的显式编程代码，但我们并不总是能够识别模型是如何从输入到输出的。研究人员将这一挑战称为机器学习的黑箱问题。

在过于气馁之前，我们必须记住，人类大脑本身就是一个黑匣子。我们并不真正知道它是如何工作的，也不能在所有抽象层次上检查它。如果我让你解剖一个大脑并指出其中的记忆，我会被贴上疯子的标签。然而，不能理解某事并不是游戏结束，而是游戏开始。

这篇文章介绍了许多支持机器学习的基本概念，但为未来的世界贸易论坛留下了很多零碎的东西。深度学习、强化学习和神经网络都可以独立存在，但希望在阅读这篇文章后，你能想象这个领域本身，并与我们每天在 TechCrunch 上报道的许多公司建立联系。

## WTF 的更多帖子是系列文章

**[WTF 是容器吗？](https://web.archive.org/web/20230130011456/https://techcrunch.com/2016/10/16/wtf-is-a-container/)**

**[搞什么鬼是诱饵？](https://web.archive.org/web/20230130011456/https://techcrunch.com/2016/09/25/wtf-is-clickbait/)**

**WTF 是一台无反光镜相机吗？**