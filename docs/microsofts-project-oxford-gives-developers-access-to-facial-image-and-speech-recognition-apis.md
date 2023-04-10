# 微软的牛津项目为开发者提供了面部、图像和语音识别 API

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/04/30/microsofts-project-oxford-gives-developers-access-to-facial-image-and-speech-recognition-apis/>

微软昨天悄悄推出了一套新的机器学习 API 测试版，名为“ [Project Oxford](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/) ”，今天这项服务的 How-Old.net 演示迅速走红。

这个网站可以让你上传人脸照片，然后自动计算出照片中人的年龄。这是一个很酷的演示——而且效果相当好(尽管正如所料，它犯了相当多的错误)。最好对它的结果有所保留，但是尽管微软的演示很有趣，但它的用例可能更倾向于试图弄清楚图像是以儿童还是成人为特征。

How-Old 使用了“牛津项目”中的部分新开发服务，但不是全部

新的 API 还允许开发者在他们的应用中添加 T2 人脸检测和识别功能。默认情况下，该服务将试图计算出用户的年龄，并将这些信息提供给开发者。

正如 Ryan Galgon，微软技术与研究部门牛津项目的高级项目经理，在今天的微软 Build 开发者大会上告诉我的，牛津和年龄检测项目是微软内部不同团队之间主要合作的结果。今天通过这项服务可以获得的大部分内容都是基于该公司在过去几年中研究的现代深度学习技术。

![SimilarFaceSearching](img/ae21abf5333a6d32aed54d01f6a41a16.png)开箱即用，该 API 还提供图像中的人脸检测、用于检查两张人脸是否属于同一个人的人脸验证，以及查找相似人脸的能力。

其他工具包括语音识别，随着时间的推移，这项服务将能够帮助开发者理解用户的意图。该项目还具有一个视觉 API，用于自动[分类图像](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/vision)并创建智能图像裁剪，总是将主题放在裁剪图像的中心。

这三项服务现已推出公测版。还有一个[第四 API](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/luis) ，它让开发者将[自定义语言理解](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/luis)构建到他们的应用程序中。

此前，微软以 Bing 品牌[提供了一套有点类似的 API。例如，Bing 提供了一个语音和翻译 API，但在大多数情况下，这些 Bing 服务比 Project Oxford 工具更基本，更侧重于搜索。Galgon 告诉我，这些 Bing APIs 更侧重于 Windows 桌面体验。另一方面，Project Oxford 工具是作为 RESTful APIs 提供的(每月限制 5000 次调用)。](https://web.archive.org/web/20230407122200/http://www.bing.com/dev/en-us/dev-center)

[Speech API](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/speech) ，顾名思义，提供语音到文本转换的语音识别服务，以及将书面文本转换为音频的文本到语音服务。更有趣的是，它还具有意图识别功能。这里的想法是让应用程序理解说话者的意图(订购墨西哥卷饼、取消航班等)。).这是由项目的[语言理解智能服务](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/luis)驱动的。

使用 image API，开发人员可以对图像进行分类，以过滤掉成人内容，或者简单地自动对图像应用标签或将其分组。该 API 还具有[光学字符识别功能](https://web.archive.org/web/20230407122200/https://www.projectoxford.ai/demo/visions#Ocr)，并允许开发人员通过识别图像中的重要内容并在您裁剪图像时将其保持在照片的中心来自动裁剪图像。

目前，这项服务是免费的。目前还不清楚微软计划何时对访问收费，但 Galgon 告诉我，该公司致力于随着时间的推移发展这些服务。

即使你不是开发者，你也可以尝试一下这些特性。

【T2![](img/26993567ce26c20c55c34446b8d2a7cc.png)