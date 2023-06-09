# 即将失败的声音 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/01/29/the-sound-of-impending-failure/>

声音是一种非常有价值的信息交流方式。大多数驾车者都熟悉皮带打滑时发出的惊人噪音。我的祖父可以用他的耳朵诊断重型轨道车的刹车问题。许多其他专家仅仅通过听它们发出的声音就能发现它们各自领域的普通机器的问题。

如果我们能找到一种自动监听的方法，我们就能更智能地日夜监控我们的世界和它的机器。我们可以实时预测引擎、铁路基础设施、石油钻井和发电厂的故障——在声音异常时通知人类。

这有可能拯救生命，但尽管机器学习取得了进步，我们仍在努力使这些技术成为现实。我们有大量的音频数据，但缺乏关键的标签。在深度学习模型的情况下，“黑盒”问题使得很难确定为什么声学异常首先被标记出来。我们仍在边缘解决实时机器学习的难题。而且声音通常包含比信号更多的噪声，限制了可以从音频数据中提取的特征。

## 声音的巨大鸿沟

机器学习领域的大多数研究人员都认为，人工智能将从地面上一步步建立起来，偶尔会有突破。按照这个配方，我们已经取消了图像字幕，征服了语音识别，但更广泛的声音仍然被机器充耳不闻。

在机器学习的许多最伟大的突破背后，隐藏着一个[精心组装的数据集。](https://web.archive.org/web/20221224200334/http://deeplearning.net/datasets/) [ImageNet](https://web.archive.org/web/20221224200334/http://image-net.org/) 用于对象识别，以及类似[语言数据联盟](https://web.archive.org/web/20221224200334/https://www.ldc.upenn.edu/)和 [GOOG-411](https://web.archive.org/web/20221224200334/https://en.wikipedia.org/wiki/GOOG-411) 用于语音识别。但是，找到一个足够的数据集来并列汽车关门声和卧室关门声是相当具有挑战性的。

“如果你正确建立模型，深度学习可以做很多事情，你只需要大量的机器数据，”帮助公司搜索音频数据的初创公司 [Deepgram](https://web.archive.org/web/20221224200334/http://www.deepgram.com/) 的首席执行官斯科特·斯蒂芬森说。“如果没有数据集，15 年前的语音识别并没有那么好。”

亚马逊土耳其机器人上狗和猫的众包标签是一回事。收集 100，000 个滚珠轴承的声音并给松动的轴承贴上标签是完全不同的事情。

虽然这些问题甚至困扰着单一用途的声学分类器，但这个领域的圣杯是一个用于识别所有声音的通用工具，而不是简单地建立一个模型来区分这些门的声音。

## 通过内省来欣赏

人类的归纳能力使我们特别擅长对声音进行分类。回想一下你最后一次听到救护车从你的公寓冲向街道的声音。即使有多普勒效应，声波频率的变化会影响你听到的警笛的音调，你也可以很容易地识别出这辆车是救护车。

https://www.youtube.com/watch?v=p-hBCcmCUPg

然而[试图自动化这一过程的研究人员必须发挥创造力。](https://web.archive.org/web/20221224200334/http://ieeexplore.ieee.org/abstract/document/5461596/)从收集运动物体信息的静止传感器中提取的特征是有限的。

缺乏[源分离](https://web.archive.org/web/20221224200334/https://en.wikipedia.org/wiki/Source_separation)会使事情更加复杂。这是一个甚至人类都在努力解决的问题。如果你曾经试图在喧闹的餐馆里挑出一个单独的桌子谈话，你就会体会到理解重叠的声音是多么困难。

[https://web.archive.org/web/20221224200334if_/https://www.youtube.com/embed/mN--nV61gDo?feature=oembed](https://web.archive.org/web/20221224200334if_/https://www.youtube.com/embed/mN--nV61gDo?feature=oembed)

视频

[英国萨里大学的研究人员](https://web.archive.org/web/20221224200334/https://www.technologyreview.com/s/537101/deep-learning-machine-solves-the-cocktail-party-problem/)能够使用深度卷积神经网络从多首歌曲的伴奏乐器中分离出人声。他们的技巧是训练 50 首歌曲的模型，这些歌曲被分成他们的乐器和声音的音轨。然后，这些曲目被切割成 20 秒的片段，以创建一个声谱图。结合完全混合歌曲的频谱图，该模型能够将新歌中的人声与伴奏乐器分开。

但用容易识别的成分分割一首五段歌曲是一回事，记录一个近 60 英尺高的人 B&W 12S90ME-C Mark 9.2 型柴油发动机的声音并要求机器学习模型将其声学特征分割成组成部分是另一回事。

## 声学拓荒者

Spotify 是更具雄心的公司之一，正在尝试将[机器学习应用于音频信号。](https://web.archive.org/web/20221224200334/http://www2.cs.uregina.ca/~gerhard/publications/TRdbg-Audio.pdf)尽管 Spotify 仍然依赖于大量其他数据，但[歌曲本身包含的信号是其广受欢迎的 Discover 功能上获得推荐的一个因素](https://web.archive.org/web/20221224200334/http://benanne.github.io/2014/08/05/spotify-cnns.html)。

音乐推荐传统上依赖于协作过滤的巧妙启发。这些基本模型通过向你推荐具有相似收听模式的其他用户播放的歌曲来避开声学分析。

![From this representation, we can see that a lot of the filters pick up harmonic content, which manifests itself as parallel red and blue bands at different frequencies. Sometimes, these bands are are slanted up or down, indicating the presence of rising and falling pitches. It turns out that these filters tend to detect human voices.](img/7e21e2621fafa51d108e9fd8d78b053b.png)

滤波器拾取不同频率的红色和蓝色波段的谐波背景。根据 Spotify 的说法，倾斜表示可以检测人声的上升和下降音调

在受控的音乐环境之外，工程师们提出了大致分为两类的解决方案。第一种我称之为“定制解决方案”模式，本质上是一家公司从客户那里收集数据，唯一的目的是识别预设的声音范围。你可以把它想象成“造一只熊”,但要贵得多，而且通常用于工业应用。

第二种方法是一种“包罗万象”的深度学习模型，可以标记任何声学异常。这些模型通常需要人在回路中手动分类声音，然后进一步训练模型寻找什么。随着时间的推移，这些系统需要的人工干预越来越少。

一家名为 [3D Signals](https://web.archive.org/web/20221224200334/https://www.3dsig.com/) 的公司，正以这两者的混合方式走向市场。该公司拥有检测旋转设备声音异常的专利。这包括电机、泵、涡轮机、齿轮箱和发电机等。

“我们建立了一个非常大规模的架构，将庞大的分布式机器舰队连接到我们的监控平台，每当这些机器开始行为不端时，算法就会突出显示，”公司首席执行官阿姆农·申菲尔德说。

![s90me-c-with-guy-10](img/46ec7f1435b4233732be8fb28d48f5b2.png)

曼 B&W 12S90ME-C Mark 9.2 型柴油机

但他们也利用现有的工程师对特别重要的问题进行分类。如果技术人员认识到问题，他们可以标记声学异常，这有助于训练学习算法，以便在未来显示这些类型的声音。

另一家名为 [OtoSense](https://web.archive.org/web/20221224200334/https://www.otosense.com/design) 的公司，实际上在其网站上提供了一个“设计实验室”。客户可以注意到他们是否有想要识别的特定声音事件的示例，该公司将帮助提供一个可以满足他们特定需求的软件平台。

预测性维护不仅是现实的，而且是随时可用的。3DSignals 和 OtoSense 等公司都瞄准了这一领域，利用商品化的物联网传感器来帮助用户无缝交换零件，以避免代价高昂的停机时间。

## 未来的机器

几年之内，我们将会有解决大量声学事件探测问题的方案。声学分析系统将能够跟踪生命周期成本，帮助企业为未来做预算。

从事噪音和振动分析的公司 [ATS 咨询](https://web.archive.org/web/20221224200334/http://www.atsconsulting.com/)的工程师香农·麦肯纳说:“联邦运输管理局强烈要求对[运输资产管理](https://web.archive.org/web/20221224200334/https://www.transit.dot.gov/TAM/rulemaking)进行状况评估。“我们认为这是帮助运输机构为其铁路系统提供状况评估指标的一种方式。”

除了车轮啸叫这样的短尾指标之外，在铁路监控的情况下，工程师们开始遇到一个相当棘手的大海捞针问题。McKenna 解释说，普通的声音信号只代表了复杂铁路系统可能面临的问题的 50%。与检查合规性不同，真正的风险管理需要一个通用的系统——你不希望一个异常情况导致灾难。

但是，我们距离能够识别任何声音的单一通用分类器还有很长的路要走。除非在算法上有所突破，否则我们将不得不分段解决这个问题。我们将需要研究人员和创始人为地下地铁系统、人类呼吸系统和关键能源基础设施的声音建立分类器，以帮助防止未来的失败。