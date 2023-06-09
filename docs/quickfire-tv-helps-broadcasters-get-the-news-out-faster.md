# QuickFire TV 帮助广播公司更快地发布新闻

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/09/08/quickfire-tv-helps-broadcasters-get-the-news-out-faster/>

无论好坏，在你的竞争对手之前获得在线视频比以往任何时候都更重要。今天在 Disrupt 战场发布，

[QuickFire.TV](https://web.archive.org/web/20230404124422/http://quickfire.tv/)

声称视频转码速度比类似服务快 10 倍，为新闻和体育组织提供视频编码，以便在从源素材上传后几分钟内在一系列设备上播放。

QuickFire 的速度是初创公司为其服务建立完整堆栈的结果，包括专门为减少代码转换时间而设计的定制硬件和软件。组成其硬件平台(该公司称之为 T-Video)的服务器中的每个机架都包含一个定制的主板，可以容纳 11 个四核英特尔酷睿 i7 处理器。这些处理器中的每一个都协调工作，由 QuickFire 称为 V-Fabric 的软件层来分配工作。此外，服务器中的每个机架都与称为 Q-Data 的另一层绑定在一起。

李在舞台上通过转码[《大巴克兔子》](https://web.archive.org/web/20230404124422/https://www.youtube.com/watch?v=YE7VzlLtp-4)展示了这个平台，他称之为“视频编辑的卡戴珊——无处不在。”在几秒钟内，他为 20 个不同的平台编码了 50 分钟的视频。

考虑到 Nvidia 等图形芯片在可以跨多个内核处理的任务中的多功能性，我预计 QuickFire 的服务器将严重依赖大型集群。但在今天的演示之前，QuickFire TV 首席执行官克雷格·李(Craig Lee)告诉我，该公司的服务器不使用任何图形处理器，除了那些内置在英特尔高端 CPU 中的处理器。在我熟悉的应用程序(视频游戏和视频编辑)中，情况并非如此，但 Lee 很坚定:“英特尔是 GPU 领域不可忽视的力量。”

[gallery ids="1054944，1054956，1054953，1054952，1054951，1054950，1054949，1054948，1054946，1054945"]

除了提供完整的堆栈之外，QuickFire 还为[提供了一套带有文档和样本代码的 API](https://web.archive.org/web/20230404124422/http://developer.quickfire.tv/)，这样视频制作团队就可以整合他们自己的工作流程和定制工具，用于上传视频和检查代码转换进度。虽然告诉 QuickFire 生成哪些配置文件(不同平台的帧速率、分辨率、颜色和音频设置)仍然需要通过快速呼叫或电子邮件聊天来完成，但只需完成一次。

免费评估期过后，QuickFire 向客户收取每分钟的基本费用:标清视频每分钟 0.10 美元(针对低带宽或移动设备上的观众)，高清视频每分钟 0.20 美元。Lee 告诉我，定期转码大型视频片段的制作团队也可以协商折扣。

[gallery ids="1053445，1053446，1053447，1053448，1053449"]

演示结束后，战场评委问了李几个问题，涉及他没有直接触及的内容。以下是他们询问的要点和李的回答(他们很快就做了这些事情):

有人在生产中使用它吗？

不，不在生产中。

**在任何给定的时刻，你们能处理多少？你一次能处理的用户有限制吗？**

关键是找到愿意为速度支付额外费用的客户—我们可以在任何云上构建。

**我在社交媒体上发布的大多数东西都只有几秒钟长。普通用户真的需要这个吗？**

我们认为目前的上传时间对于年轻用户来说太长了——他们只是不想等几个小时或一夜才能在 YouTube 上看到他们的视频。

你有内置上传到其他平台的系统吗？我可以将转码作业设置为立即转到 YouTube、Vimeo 等等吗？

我们是常规视频工作流程的一部分，只要告诉我们它需要去哪里，我们就会对它进行代码转换。我们没有内容管理系统，我们只是为您的视频做好准备，无论它们需要放在哪里。