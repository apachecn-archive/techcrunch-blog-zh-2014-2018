# 谷歌开源谷歌照片搜索、智能回复等背后的机器学习技术 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/11/09/google-open-sources-the-machine-learning-tech-behind-google-photos-search-smart-reply-and-more/>

谷歌今天表示，它正在开发机器学习技术，该技术为其许多产品提供动力，包括谷歌照片搜索、谷歌应用程序中的语音识别以及新推出的电子邮件应用程序收件箱的“[智能回复”功能](https://web.archive.org/web/20221208142057/https://beta.techcrunch.com/2015/11/03/with-smart-reply-googles-inbox-can-now-respond-to-emails-for-you-automatically/#.s2agxy:taaV)。这项名为 [TensorFlow](https://web.archive.org/web/20221208142057/http://tensorflow.org/) 的技术有助于让应用程序变得更智能，谷歌表示，它比第一代系统强大得多——使该公司建立和训练神经网络的速度比以前快了五倍。

该公司解释说，对谷歌来说，这意味着它能够更快地改进产品。

TensorFlow 最初是由谷歌机器智能研究组织内谷歌大脑团队的研究人员和工程师开发的一个项目，目的是进行机器学习和深度神经网络研究。谷歌表示，这项技术也适用于许多其他领域。

用更专业的术语来说，深度学习框架既是一个可以在 CPU、英伟达 GPU、Android、iOS 和 OS X 上运行的生产级 C++后端，也是一个与 Numpy、iPython 笔记本和其他基于 Python 的工具相接口的 Python 前端，[在他的 Google+个人资料中写道](https://web.archive.org/web/20221208142057/https://plus.google.com/+VincentVanhoucke/posts/4VFgjmRHnkQ) Vincent Vanhoucke，大脑团队的技术主管和经理。

任何可以表达为计算流图的计算，都可以用 TensorFlow 来计算。谷歌表示，任何基于梯度的机器学习算法都将受益于 TensorFlow 的[自动微分](https://web.archive.org/web/20221208142057/https://en.wikipedia.org/wiki/Automatic_differentiation)和一流的优化器套件。

“TensorFlow 是我们在谷歌大脑团队中每天使用的东西，虽然它仍处于早期阶段，还有许多粗糙的边缘需要解决，但我很高兴有机会围绕它建立一个研究人员、开发人员和基础设施提供商的社区，”Vanhoucke 说。

机器学习的目标是建立一种类似于人脑的技术，但无论如何，这种技术还不存在。

在宣布这一消息的谷歌博客文章中，由首席执行官桑德尔·皮帅撰写，他解释说，通过开源技术，希望它将加速对机器学习的研究，这将使整个社区受益，并使技术更好地工作。正如皮查伊指出的那样，即使是当今最好的系统也很难做到一个 4 岁的孩子能做到的事情——比如只看了几个例子就知道一只恐龙的名字，或者理解“我看到大峡谷飞往芝加哥”这句话并不意味着空中真的有一个飞行的峡谷。

此外，该公司认为 TensorFlow 有能力在研究中发挥作用，以理解复杂的数据，例如蛋白质折叠或处理天文学数据。

TensorFlow 的有趣之处在于它使研究人员和开发人员能够在机器学习技术上进行合作。TensorFlow 让研究人员测试新想法，并在工作时将它们转移到产品中，而不必重新编写代码，而不是为每个小组提供单独的工具。这可以加快产品的改进，当然，通过让更大的机器学习社区也能这样做，谷歌也将受益于开源技术带来的创新步伐的加快。随着这项技术被集成到更多的产品中并得到改进，这最终会提高谷歌的底线。

TensorFlow 可以识别照片和视频中的内容，理解语音，阅读和理解书面文本(在一定程度上)等等。

后一个功能是“智能回复”的动力，这是谷歌电子邮件应用 Inbox 为你的电子邮件创建自动回复的一种方式——这是一个易于理解的机器学习增强我们日常使用的产品(如电子邮件)的潜力的例子。智能回复阅读电子邮件的内容，然后在屏幕底部建议您可以用来回复的短语。例如，你用得越多，它就知道你对谁说“是”和“不是”。

谷歌表示，TensorFlow 目前被用于其许多最引人注目的产品中，包括谷歌照片中的图像搜索、语音识别系统、Gmail、谷歌搜索等。

谷歌表示，它使用了 2011 年开发的早期系统 DistBelief 来证明“猫”等概念可以从未标记的 YouTube 图像中学习，将谷歌应用程序中的语音识别能力提高了 25%，并在谷歌照片中建立图像搜索。dist faith 还训练了盗梦空间模型，该模型在 2014 年赢得了 Imagenet 的[大规模视觉识别挑战](https://web.archive.org/web/20221208142057/http://googleresearch.blogspot.com/2014/09/building-deeper-understanding-of-images.html)，并在[自动图像字幕](https://web.archive.org/web/20221208142057/http://googleresearch.blogspot.com/2014/11/a-picture-is-worth-thousand-coherent.html)和 [DeepDream](https://web.archive.org/web/20221208142057/http://googleresearch.blogspot.com/2015/06/inceptionism-going-deeper-into-neural.html) 的实验中使用。

但该公司表示，DistBelief 有局限性——“它的目标仅限于神经网络，难以配置，并且与谷歌的内部基础设施紧密耦合——这使得它几乎不可能在外部分享研究代码，”该公司在其研究博客[上的另一份声明中表示，该声明由谷歌高级研究员杰夫·迪恩(Jeff Dean)和技术主管拉杰特·蒙加(Rajat Monga)撰写。](https://web.archive.org/web/20221208142057/http://googleresearch.blogspot.com/2015/11/tensorflow-googles-latest-machine_9.html)

TensorFlow 旨在解决这些缺点。

“TensorFlow 是通用的、灵活的、可移植的、易于使用的、完全开源的。我们在提高 dist faith 的速度、可扩展性和生产就绪性的同时增加了所有这些功能——事实上，在某些基准测试中，TensorFlow 的速度是 dist faith 的两倍，”该公告称。

谷歌不是唯一一家建立机器学习系统的主要科技公司。IBM Watson、[亚马逊机器学习](https://web.archive.org/web/20221208142057/https://aws.amazon.com/machine-learning/)、 [Azure 机器学习](https://web.archive.org/web/20221208142057/https://beta.techcrunch.com/2015/02/18/microsoft-officially-launches-azure-machine-learning-big-data-platform/)是市场上其他著名的名字。

[YouTube https://www.youtube.com/watch?v=oZikw5k_2FM]