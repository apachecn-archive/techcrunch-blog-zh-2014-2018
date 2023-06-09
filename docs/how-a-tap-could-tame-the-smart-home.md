# 水龙头如何驯服智能家居

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/09/how-a-tap-could-tame-the-smart-home/>

对于与各种联网设备进行交互的头痛问题，这里有一个新颖的解决方案:卡内基梅隆大学的研究人员设计了一个系统，让智能手机用户对着物联网设备点击他们的手机，以便在屏幕上自动加载上下文菜单——从而使他们不必四处寻找正确的应用程序来控制每台设备。或者摆弄实际的物理按钮并试图浏览不太友好的菜单。

因此，换句话说，正如 CMU 研究员 Chris Harrison 所说，“不用再通过手机上无尽的应用程序页面来控制你所谓的‘智能家居’”。

这个系统叫做德乌斯·埃姆·玛奇纳(看看他们在那里做了什么？)，利用日常电器发出电磁噪声的事实来驱动设备分类器——他们正在使用配备有电磁传感器的智能手机，该传感器可以检测它停留在哪个物联网设备上——从而将上下文功能推送到智能手机屏幕上，因此它可以是一个动态控制设备。

“没有理由不能在未来几年内集成到智能手机中，”哈里森说，他预计电磁感应技术的小型化将为未来的商业部署铺平道路。

虽然 CMU 未来接口集团的研究人员之前已经向展示了运行在可穿戴设备上的类似电磁感应系统——也用于为其他设备的上下文感知提供动力——但在最新的研究场景中，使用智能手机作为控制设备意味着用户可以获得更丰富的菜单，从而支持更多的控制功能。

哈里森证实，最新的电磁感应研究是早期可穿戴设备项目的延伸，他告诉 TechCrunch，它已经提高了精确度，而且“更小，更独立”。但最大的不同是探索了“非常不同的外形”，以及如何在应用层利用它。

“这并不是说一个项目/技术比另一个更好，更多的是因为转换外形打开了不同的互动机会，”他说。“特别是，与智能手表不同，你可以在智能手机上执行不同的活动。与其说是配件，不如说是工具。”

在 T2 的一篇关于新研究的论文中，该团队写道:

> 我们提出了一种方法，用户只需将智能手机轻触设备，即可发现并快速利用上下文功能。为了实现这一点，我们的原型智能手机可以识别与未测试设备的物理接触，并调用设备特定的接口。我们的用户研究表明准确率很高，在 17 种设备中识别准确率达到 98.8%。最后，为了强调我们系统的直接可行性和实用性，我们构建了 12 个示例应用程序，包括 6 个全功能的端到端演示

下面的视频展示了研究人员为演示传感系统而开发的应用程序的例子——包括控制恒温器；配置路由器；只需按一下打印按钮，即可打印移动设备屏幕上的文档；从手机向台式电脑发送文本；还有更多。

研究人员创建了一个后台 Android 服务，与他们的物联网设备分类器一起运行，为某些应用程序将所谓的“上下文魅力”推送到屏幕上——也就是当手机触摸支持的设备时出现在应用程序右边缘的小浮动按钮，它可以执行命令(例如将视频内容流式传输到智能电视的“施展魅力”，或者打印屏幕上的内容的打印按钮)。

“我们预计，未来的智能家电应用程序将在安装时向 charm system 服务注册其设备的 EM 签名和一组动词，这将使现有应用程序能够立即利用用户环境中的设备和装置。这类似于当前的应用程序注册 Android“共享”处理程序来支持系统范围的内容共享，例如，社交媒体，”他们写道。

哈里森补充说,“上下文魅力”的想法是为两件事同时发生的地方开发的——比如在手机上阅读 PDF，然后在打印机上点击它。“这突然在手机和设备之间打开了一个更丰富的协同活动集——而现在，你的手机真的不知道它周围发生了什么或它应该显示什么功能，”他补充道。

在他们的论文中，研究人员讨论了该系统的总体局限性，强调了物联网设备拥有开放 API 的必要性，并指出:“我们最初开始为我们列表中的所有联网设备生产全栈实现。然而，我们被其中几个缺乏公共 API 所困扰。此外，即使 API 可用，一些也是供应商锁定的(例如，Apple TV 演员表 API 只对苹果设备开放)。为了让未来的物联网产生真正的影响，开放 API 是一个强烈的要求。在那之前，我们的系统将受到无法与所有智能设备对话的限制。”

其他限制包括难以识别同一设备的多个实例(例如，多于一个连接的恒温器)；以及来自电力线噪声的外部干扰，这可能混淆设备分类器。如果设备真正断电，传感系统也无法工作——尽管研究人员指出，低功耗或睡眠模式仍可能使物联网对象可被检测到。

这项研究于本周在丹佛举行的 ACM CHI 会议上发表。CMU 还在会议上展示了另一项有趣的界面研究——使用导电喷漆和电极阵列将任何表面变成触摸敏感表面。