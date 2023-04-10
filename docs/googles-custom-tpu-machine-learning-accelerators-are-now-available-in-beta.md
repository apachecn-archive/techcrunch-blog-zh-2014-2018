# 谷歌定制的 TPU 机器学习加速器现已推出测试版 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/12/googles-custom-tpu-machine-learning-accelerators-are-now-available-in-beta/>

# 谷歌定制的 TPU 机器学习加速器现已推出测试版

谷歌的[张量处理单元](https://web.archive.org/web/20221210055524/https://cloud.google.com/blog/big-data/2017/05/an-in-depth-look-at-googles-first-tensor-processing-unit-tpu) (TPUs)，该公司为其 [TensorFlow](https://web.archive.org/web/20221210055524/https://www.tensorflow.org/) 框架编写的运行机器学习工作负载的定制芯片[现在](https://web.archive.org/web/20221210055524/https://cloudplatform.googleblog.com/2018/02/Cloud-TPU-machine-learning-accelerators-now-available-in-beta.html) [可供开发者使用](https://web.archive.org/web/20221210055524/https://cloud.google.com/tpu/)。

这些谷歌设计的芯片的承诺是，它们可以运行特定的机器学习工作流，速度远远快于大多数开发人员今天使用的标准 GPU。对于谷歌来说，这些 TPU 的优势之一是它们也使用更少的电力，开发者可能不太关心这一点，但这使谷歌能够以更低的成本提供这项服务。

该公司在九个月前的 I/O 开发者大会上首次发布了云处理器(并向有限数量的开发者和研究人员开放)。每个云 TPU 都有四个定制的 ASICs，64 GB 的高带宽内存。据谷歌称，单块 TPU 主板的最高性能为 180 万亿次浮点运算。

[![](img/8f9a359bb77443929afa2322e7274c4d.png)](https://web.archive.org/web/20221210055524/https://beta.techcrunch.com/wp-content/uploads/2018/02/tpu-v2-1-max-1000x1000.png)

已经使用 TensorFlow 的开发人员无需对其代码进行任何重大更改即可使用该服务。不过，就目前而言，云 TPU 还不能通过点击一个按钮来实现。“为了管理访问”，正如谷歌所说，开发者必须申请云 TPU 配额，并描述他们想用这项服务做什么。一旦他们进入，使用费将按每小时每云 TPU 6.50 美元计费。相比之下，在美国使用标准的特斯拉 P100 GPU 的费用是每小时 1.46 美元，尽管这里的最高性能约为 FP16 性能的 21 万亿次浮点运算。

谷歌在机器学习方面的声誉肯定会为这些云 TPU 带来大量新用户。然而，从长远来看，可能同样重要的是，这给了谷歌云一种区别于 AWS 和 Azure 的方式。毕竟，在很大程度上，每个人现在都提供相同的基本云计算服务，容器的出现使得将工作负载从一个平台转移到另一个平台变得更加容易。通过 TensorFlow 和 TPUs 的结合，谷歌现在可以提供一种短期内很少有人能与之匹敌的服务。