# 谷歌的 AutoML 让你无需编码就能训练定制的机器学习模型

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/01/17/googles-automl-lets-you-train-custom-machine-learning-models-without-having-to-code/>

谷歌今天[宣布](https://web.archive.org/web/20230312044627/https://www.blog.google/topics/google-cloud/cloud-automl-making-ai-accessible-every-business/)阿尔法推出 [AutoML Vision](https://web.archive.org/web/20230312044627/https://cloud.google.com/automl/) ，这是一项帮助开发者——包括那些没有机器学习(ML)专业知识的人——构建定制图像识别模型的新服务。虽然谷歌计划将 AutoML 品牌下的定制 ML 模型生成器扩展到其他领域，但该服务目前仅支持计算机视觉模型，但你可以预计该公司将为其所有标准 ML [构建模块](https://web.archive.org/web/20230312044627/https://cloud.google.com/products/machine-learning/)推出类似版本的 AutoML(想想语音、翻译、视频、自然语言识别等)。).

谷歌表示，这里的基本想法是允许几乎任何人带来他们的图像，上传它们(并导入他们的标签或在应用程序中创建它们)，然后让谷歌的系统自动为他们创建一个客户机器学习模型。该公司表示，例如，迪士尼已经使用该系统使其在线商店的搜索功能更加强大，因为它现在可以找到所有与闪电麦昆相似的产品，而不仅仅是那些你最喜欢的会说话的赛车被标记在文本描述中的产品。

[![](img/b1e0069a4886019be0f2a458800e54b3.png)](https://web.archive.org/web/20230312044627/https://techcrunch.com/wp-content/uploads/2018/01/cloud_auto_ml.gif)

从导入数据到标记数据和训练模型的整个过程都是通过拖放界面完成的。不过，我们这里不是在谈论类似于微软 Azure ML studio 的东西，在那里你可以使用类似雅虎 Pipes 的界面来构建、训练和评估模型。相反，谷歌选择了一个系统来处理所有的艰苦工作，并为你训练和调整你的模型。

众所周知，如今企业几乎不可能雇佣机器学习专家和数据科学家。需求太大，而供给不足。

“人工智能和机器学习仍然是一个进入门槛很高的领域，需要的专业知识和资源很少公司能够独自负担得起，”谷歌人工智能/人工智能首席科学家费-李非在本周早些时候的一次新闻发布会上说。如果你假设今天有大约 100 万数据科学家，那么这差不多就是能够使用你的工具的人数。“今天，虽然人工智能为企业提供了无数好处，但开发一个定制模型往往需要罕见的专业知识和广泛的资源。”

[图库 ids="1587477，1587471，1587472，1587473，1587474，1587475，1587476，1587478，1587479，1587480，1587481，1587468，1587469，1587470"]

谷歌认为 AutoML 是市场上唯一的同类系统。然而，公平地说，已经有像 Clarif.ai 和其他服务在采取类似的方法。事实上，微软的[认知服务](https://web.archive.org/web/20230312044627/https://azure.microsoft.com/en-us/services/cognitive-services/)也将很乐意允许你定制其预训练的[模型，用于视觉](https://web.archive.org/web/20230312044627/https://www.customvision.ai/)、[语音识别](https://web.archive.org/web/20230312044627/https://docs.microsoft.com/en-us/azure/cognitive-services/custom-speech-service/cognitive-services-custom-speech-home)和[决策](https://web.archive.org/web/20230312044627/https://docs.microsoft.com/en-us/azure/cognitive-services/custom-decision-service/custom-decision-service-overview)(尽管所有这些都还在预览阶段)。

为了获得 AutoML Visions 的访问权限，开发者目前必须[申请访问权限](https://web.archive.org/web/20230312044627/https://services.google.com/fb/forms/cloudautomlalphaprogram/)。该公司尚未分享任何定价信息，但有可能它会对训练模型收取一笔费用，然后对通过其 API 访问模型收取另一笔费用。