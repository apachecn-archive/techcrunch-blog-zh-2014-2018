# 微软希望帮助开发者将他们的人工智能模型带到桌面上

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/03/07/microsoft-wants-to-help-developers-bring-their-ai-models-to-the-desktop/>

微软今天宣布了其面向 Windows 开发者的人工智能平台，这是一套新的工具，将很快帮助开发者将他们在云中训练的机器学习模型带到他们的桌面应用程序中。Windows 10 中的人工智能平台将与 Windows 的下一个主要版本一起推出，它将利用本地机器上的 GPU，并允许开发人员实时运行他们的模型，而无需往返于云端。

“从人工智能的角度来看，我们正在构建的东西真正完成了微软的故事，”微软合作伙伴集团项目经理 Kam VedBrat 告诉我。过去，微软谈论了很多关于它在云中的机器学习基础设施以及围绕它建立的工具。有了这个，开发人员现在可以使用他们选择的框架在云中轻松地构建他们的模型，然后使用 Visual Studio 和微软为此构建的一些其他工具轻松地将这些模型与他们的桌面应用程序集成。

这其中的核心是由微软、脸书和亚马逊支持的 T2 项目 Onnx T1。它允许开发人员将 Caffe2、PyTorch、CNTK 和其他模型转换成 Onnx 格式，以便在必要时在框架之间移动它们。

微软还将允许开发者使用 [Azure 定制视觉服务](https://web.archive.org/web/20221208101520/https://azure.microsoft.com/en-us/services/cognitive-services/custom-vision-service/)构建图像识别模型，并将其导出用于 Windows ML。与使用传统框架不同，开发人员不需要了解构建机器学习模型的复杂性。他们需要做的就是给服务提供他们标记的训练数据。

这些型号然后利用任何给定机器中可用的硅，这很可能意味着 DirectX 12 显卡，或者如果没有，CPU。但该平台也将提供一个灵活的 API 来访问其他硬件，例如，包括未来的英特尔 Movidius 视觉处理单元。

微软公司副总裁凯文·加洛告诉我，这样做的好处不仅是降低了延迟，增加了用户数据的隐私性，还降低了成本。毕竟，在云中运行这些模型确实会产生成本，而且成本会迅速增加。但是，当它们在桌面上运行时，这就不是问题了。

从 Visual Studio 15.7 的下一个预览版开始，开发人员只需将 ONNX 文件添加到他们的通用 Windows 平台(UWP)应用程序中，Visual Studio 就会为该项目生成一个模型界面。微软还将为以前版本的 Visual Studio 提供工具，并将这一功能添加到用于人工智能的 Visual Studio 工具中。