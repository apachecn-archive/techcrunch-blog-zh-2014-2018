# 谷歌在 Android 8.1 开发者预览版中引入神经网络 API 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/10/25/google-introduces-neural-networks-api-in-developer-preview-of-android-8-1/>

# 谷歌在 Android 8.1 的开发者预览版中引入了神经网络 API

今天，谷歌开始为 Android Oreo 开发新的开发者测试版(8.1)。

这里的一大亮点是新的[神经网络 API](https://web.archive.org/web/20230321044908/https://developer.android.com/ndk/guides/neuralnetworks/index.html) ，它为手机带来了硬件加速推理，可以快速执行之前训练过的机器学习模型。通过减少网络延迟和负载，同时将更多敏感数据保留在设备上，将这些计算带到边缘可以为最终用户带来很多效用。

当允许手机上的应用程序做诸如分类图像或学习你的习惯如何预测行为之类的事情时，这可以派上用场。谷歌表示，他们将神经网络 API 设计为 TensorFlow Lite、Caffe2 等框架的“基础层”。

【T2![](img/837fa603d73834519dfa6c1deb39c721.png)

如果可行的话，API 可以利用设备上的特殊人工智能芯片——或者如果这是唯一的选择，就退回到 CPU。谷歌的新 Pixel 2 手机[采用了这样一种特殊的芯片](https://web.archive.org/web/20230321044908/https://techcrunch.com/2017/10/17/googles-first-custom-consumer-chip-is-the-secret-behind-the-pixel-2s-camera-performance/)(Pixel 视觉核心)，谷歌此前表示，它计划在 8.1 预览版上线后立即启用它(所以今天……)。

虽然神经网络 API 专注于将更多工作放在用户的设备上，但谷歌也在 8.1 中引入了一些针对 Android Go 的优化，这应该有助于开发人员针对更基本的智能手机的轻量级 Android 版本的用户，这是谷歌在今年 5 月的 I/O 上宣布的。

Go 是一款低规格、连接性差的手机。此更新主要针对运行内存小于 1GB 的设备进行内存优化；如果运行 8.1 或更高版本，开发人员还可以根据设备的系统内存将更新分发到设备上。

除此之外，8.1 开发者预览版将为自动填充带来一些更新，因此密码管理员可以更容易地使用该框架。这些更新都是对预期的错误补丁和安全补丁的补充。

Android 8.1 要到 12 月份才会面向消费者，但如果你是一名开发者，你现在就可以开始测试了。