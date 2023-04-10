# 来自“硅谷”的非热狗应用背后的工程师在 AI TechCrunch 上花了很多心思

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/06/28/thinking-about-hotdogs/>

# 来自“硅谷”的非热狗应用背后的工程师对人工智能投入了很多思考

对于像 HBO 的硅谷这样的节目来说，展示一个机器学习应用程序是很容易的，该应用程序通过一些聪明的后处理对热狗进行分类——放入一些虚假的静态截图，然后就可以收工了。如果这个团队想创建一个真正的应用程序用于品牌推广，他们可以用黑客马拉松的方式把一些 API 串在一起，然后继续下一个愚蠢的恶作剧。但值得称赞的是，蒂姆·安格拉德(Tim Anglade)是病毒式恶搞应用程序 Not Hotdog 背后的工程师，[可能比本周在沙丘上推介的至少一家“人工智能”初创公司投入了更多的思考。](https://web.archive.org/web/20230218154843/https://medium.com/@timanglade/how-hbos-silicon-valley-built-not-hotdog-with-mobile-tensorflow-keras-react-native-ef03260747f3)

Anglade 没有使用类似谷歌的云视觉 API 的东西，而是实际上进入了杂草中，用 TensorFlow 和 Keras 进行实验。因为 Hotdog 不必在本地移动设备上运行，所以 Anglade 面临着一系列及时的挑战，任何在移动设备上开发应用程序的机器学习开发者都可能会遇到这些挑战。

[在一篇中期文章](https://web.archive.org/web/20230218154843/https://medium.com/@timanglade/how-hbos-silicon-valley-built-not-hotdog-with-mobile-tensorflow-keras-react-native-ef03260747f3)中，安格雷德讨论了他最初是如何利用笔记本电脑上连接的 eGPU 对几千张热狗图像进行迁移学习来重新训练盗梦空间架构的。但即便如此，他的模型过于臃肿，无法在移动设备上可靠运行。

![](img/85c2abb0f6a2ee4c9225f20c7864aedf.png)

蒂姆·安格拉德

所以他试着使用 SqueezeNet，一个更精简的网络，运行时需要更少的内存。不幸的是，尽管它的尺寸很小，但它的性能受到过度和欠配合的影响。

即使给定了一个大的热狗数据集，而不是热狗训练图像，该模型也不能完全掌握热狗的抽象概念，而是似乎使用了糟糕的启发式方法作为拐杖(红酱=热狗)。

幸运的是，谷歌刚刚发表了他们的 [MobileNets 论文](https://web.archive.org/web/20230218154843/https://arxiv.org/abs/1704.04861)，提出了一种在移动设备上运行神经网络的新方法。谷歌提出的解决方案在臃肿的 Inception 和脆弱的 SqueezeNet 之间提供了一个中间地带。更重要的是，它允许 Anglade 轻松调整网络，以平衡准确性和计算可用性。

Anglade 使用 GitHub 的开源 Keras 实现作为起点。然后，他做了大量的修改来简化模型，并针对一个特定的用例进行优化。

最终的模型在 150，000 幅图像的数据集上进行训练。大多数，147，000 张图片不是热狗，而 3，000 张图片是热狗。这个比例是有意反映出世界上大多数物体都不是热狗的事实。

你可以在这里查看故事的其余部分，安格雷德在这里详细讨论了他的所有方法。他继续解释了一种有趣的技术，在提交到应用商店后，使用 CodePush 将更新实时注入到他的神经网络中。虽然这个应用程序完全是一个笑话，但安格雷德在最后节省了时间，就 UX/UI 的重要性以及他在培训过程中必须考虑的偏见进行了深刻的讨论。