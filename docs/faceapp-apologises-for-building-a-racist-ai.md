# FaceApp 为构建种族主义 AI 道歉

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/04/25/faceapp-apologises-for-building-a-racist-ai/>

如果所有的算法偏见都像这样容易发现就好了:FaceApp，一个照片编辑应用程序，[使用神经网络以照片写实的方式编辑自拍](https://web.archive.org/web/20230406160904/https://techcrunch.com/2017/02/08/faceapp-uses-neural-networks-for-photorealistic-selfie-tweaks/)，已经为建立一个种族主义算法道歉。

该应用程序允许用户上传自拍或面部照片，并提供一系列滤镜，然后可以应用于图像，以微妙或彻底改变其外观——其外观改变效果包括衰老甚至改变性别。

问题是该应用程序还包括一个所谓的“性感”过滤器，这个过滤器是种族主义的。正如[的用户指出的](https://web.archive.org/web/20230406160904/https://twitter.com/tweeterrance/status/854766266094985216)，这种滤镜是为了提亮肤色，以达到其所谓的“美化”效果。你可以在上面奥巴马总统前后的照片中看到滤镜。

在一份为种族主义算法道歉的电子邮件声明中，FaceApp 的创始人兼首席执行官雅罗斯拉夫·冈查罗夫告诉我们:“我们对这个毫无疑问非常严重的问题深感抱歉。这是由训练集偏差引起的底层神经网络的不幸副作用，而不是有意的行为。为了缓解这个问题，我们重新命名了效果，以排除任何与之相关的积极内涵。我们还在努力完成修复工作，应该很快就会完成。”

正如[卫报](https://web.archive.org/web/20230406160904/https://www.theguardian.com/technology/2017/apr/25/faceapp-apologises-for-racist-filter-which-lightens-users-skintone)早些时候指出的，这款应用在最近几周人气飙升——这或许促使 FaceApp 意识到过滤器有问题。

FaceApp 已经暂时将令人不快的过滤器的名称从“hotness”改为“spark”，尽管在一个非种族主义的替代品准备推出之前，将它从应用程序中完全删除会更聪明。可能他们被这款应用的病毒式流行分散了注意力(它显然每天增加大约 70 万用户)。

虽然支持 FaceApp 效果的底层人工智能技术包括来自一些开源库的代码，如谷歌的 TensorFlow，但冈查罗夫向我们证实，用于训练“热度”过滤器的数据集是它自己的，而不是公共数据集。所以我们无法逃避责任。

坦率地说，很难找到一个更好的(直观的)例子来说明算法中隐含的偏见风险。机器学习模型的好坏取决于它所输入的数据——在 FaceApp 的情况下，莫斯科团队显然没有在足够多样化的数据集上训练他们的算法。我们至少可以感谢他们以如此具有视觉冲击力的方式说明了潜在的算法偏差问题。

随着人工智能控制越来越多的系统，迫切需要对[算法问责](https://web.archive.org/web/20230406160904/https://techcrunch.com/2016/10/12/ai-accountability-needs-action-now-say-uk-mps/)进行全面质询，并开发健壮的系统以避免将人类偏见嵌入我们的机器。自主技术并不意味着“不受人类缺陷的影响”，任何试图宣称并非如此的开发者都是在试图兜售谎言。