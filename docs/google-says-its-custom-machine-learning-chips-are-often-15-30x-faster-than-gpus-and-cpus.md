# 谷歌表示，其定制的机器学习芯片通常比 GPU 和 CPU 快 15-30 倍

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/04/05/google-says-its-custom-machine-learning-chips-are-often-15-30x-faster-than-gpus-and-cpus/>

# 谷歌表示，其定制的机器学习芯片通常比 GPU 和 CPU 快 15-30 倍

谷歌开发了自己的定制芯片来加速其机器学习算法，这已经不是什么秘密了。该公司在 2016 年 5 月的 I/O 开发者大会上首次披露了这些被称为张量处理单元(TPU)的芯片，但它从未透露关于它们的所有细节，只是说它们是围绕该公司自己的 [TensorFlow](https://web.archive.org/web/20230407094606/https://www.tensorflow.org/) 机器学习框架进行优化的。今天，它第一次分享了[关于该项目的更多细节](https://web.archive.org/web/20230407094606/https://drive.google.com/file/d/0Bx4hafXDDq2EMzRNcy1vSUxtcEk/view)和[基准](https://web.archive.org/web/20230407094606/https://cloudplatform.googleblog.com/2017/04/quantifying-the-performance-of-the-TPU-our-first-machine-learning-chip.html)。

如果你是一名芯片设计师，你可以在谷歌的论文中找到所有关于 TPU 如何工作的血淋淋的细节。然而，这里最重要的数字是基于谷歌自己的基准测试(值得记住的是，这是谷歌评估自己的芯片)，在执行谷歌的常规机器学习工作负载时，TPU 平均比标准 GPU/CPU 组合(在这种情况下，英特尔 Haswell 处理器和 Nvidia K80 GPUs)快 15 至 30 倍。由于功耗在数据中心也很重要，TPU 还提供了 30 到 80 倍的万亿次/瓦(随着未来使用更快的内存，这些数字可能会增加)。

[![](img/d891530fa621564063bdbedc6845ac9a.png)](https://web.archive.org/web/20230407094606/https://techcrunch.com/wp-content/uploads/2017/04/2017-04-05_1014.png)

顺便说一下，值得注意的是，这些数字是关于在生产中使用机器学习模型的——而不是关于首先创建模型。

谷歌还注意到，虽然大多数架构师为[卷积神经网络](https://web.archive.org/web/20230407094606/http://cs231n.github.io/convolutional-networks/)(例如，一种非常适合图像识别的特定类型的神经网络)优化他们的芯片。然而，谷歌表示，这些网络仅占其数据中心工作负载的大约 5%，而其大多数应用程序都使用[多层感知机](https://web.archive.org/web/20230407094606/https://en.wikipedia.org/wiki/Multilayer_perceptron)。

谷歌表示，早在 2006 年，它就开始研究如何在其数据中心使用 GPU、FPGAs 和定制 ASICS(本质上就是 TPU)。然而，当时并没有多少应用程序能够真正受益于这种特殊的硬件，因为它们所需的大多数繁重工作负载都可以利用数据中心中已经可用的多余硬件。谷歌论文的作者写道:“2013 年，当我们预测 DNNs 可能变得如此受欢迎，以至于它们可能会使我们的数据中心的计算需求增加一倍，而用传统的 CPU 来满足这些需求将非常昂贵。”“因此，我们启动了一个高优先级项目，以快速生产用于推理的定制 ASIC(并购买现成的 GPU 用于培训)。”谷歌的研究人员说，这里的目标是“将性价比提高到 GPU 的 10 倍。”

谷歌不太可能在自己的云之外提供 TPU，但该公司指出，它希望其他人能够借鉴它的经验，“打造继任者，将标准提高到更高的水平。”

[![](img/b5a5542b5f8b1492d824623f9bc8849b.png)](https://web.archive.org/web/20230407094606/https://techcrunch.com/wp-content/uploads/2017/04/2017-04-05_1011.png)