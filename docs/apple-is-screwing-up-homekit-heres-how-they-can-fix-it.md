# 苹果在搞砸 HomeKit 以下是他们解决问题的方法 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/09/30/apple-is-screwing-up-homekit-heres-how-they-can-fix-it/>

丹尼尔·康拉德撰稿人

丹尼尔是

[Beep Networks](https://web.archive.org/web/20221006185144/http://www.beepnetworks.com/)

，是谷歌 Android 和 Access 团队的早期产品经理。

More posts by this contributor

当设备协同工作时，物联网的真正魔力就会显现。

当你的 iPhone 上的 Siri 可以调整你的恒温器或确认你锁了后门时，这将是神奇的；当你的门锁可以告诉你的音响系统你在家，你甚至不必按下按钮就可以开始播放音乐。

这并不是我们今天生活的现实，因为大多数设备都无法相互通信。没有共同语言，这种神奇就不可能发生。

苹果(通过 [HomeKit](https://web.archive.org/web/20221006185144/http://www.apple.com/ios/home/) )和谷歌(通过[与 Nest](https://web.archive.org/web/20221006185144/https://nest.com/works-with-nest/) 合作)已经引入了支持这种类型通信的程序。作为两大主流手机平台的所有者，它们都有能力为室内设备通信设定标准。

然而，领养 Nest 的工作比 HomeKit 领先了好几光年。看看这些数字:[苹果网站](https://web.archive.org/web/20221006185144/http://www.apple.com/us/shop/accessories/all-accessories/home-automation?page=1#!&f=homekitcompatible&fh=459b%2B4559)目前拥有来自 7 家制造商的 HomeKit- 兼容设备。[与嵌套](https://web.archive.org/web/20221006185144/https://workswith.nest.com/products)页面显示 95。

Nest 可以连接洗衣机、宠物喂食器和婴儿监视器。HomeKit 只适用于飞利浦灯，没有其他功能。

苹果制造设备已经有很长时间了。他们在一个比 Nest 多得多的家里，他们的零售店应该给他们在吸引合作伙伴方面带来巨大的优势。此外，连接到 iPhone 应该很容易。那么为什么 Nest 的设备合作伙伴要多一个数量级呢？

## 硬件慢，软件快

方法的根本区别在于硬件和软件。苹果要求硬件集成。Nest 在云中进行集成。

我们的团队制造了首批连接到 Nest 的设备之一。一名工程师花了几天时间完成了集成和认证测试流程。几乎所有的事情都发生在云中，而不是在用户的本地 Wi-Fi 网络上。

我们得到了 Nest 团队的大力支持，或者他们的文档是公开的、优秀的，这都没有坏处。或者那个 [Firebase](https://web.archive.org/web/20221006185144/https://firebase.google.com/) 很牛逼。(谷歌实际上[收购了](https://web.archive.org/web/20221006185144/https://beta.techcrunch.com/2014/10/21/google-acquires-firebase-to-help-developers-build-better-realtime-apps/)Firebase——也许只是为了让 Nest 的作品更好？)

苹果做的事情完全不同。

你必须申请访问 MFi 开发者计划，才能查看关于 HomeKit 硬件集成的文档。说真的，你必须等待数周的批准，才能阅读 HomeKit 设备要求。

苹果公司要求在你的硬件上安装认证芯片，你只能从他们那里购买。现有产品不能连接到 HomeKit 而不改变其电气设计。

> 这就像在一个有电子邮件的世界里，他们要求我们使用传真机。

你还必须和他们认可的制造商之一一起生产你的产品。如果您当前的制造商不在列表中，您必须将生产线移至新工厂。你必须在苹果认可的实验室中测试和认证你的设备。我知道只有少数几个——我在旧金山的一个朋友不得不把他的设备送到英国进行测试。

我甚至听说苹果会检查你的包装，以确保颜色不会与他们的品牌计划相冲突。老实说，我选择不相信那是真的——但也许是真的。

## 集成属于云

最重要的是，苹果要求大部分设备到设备的集成发生在本地 Wi-Fi 网络上——而不是与服务器对话，你的设备通过本地 Wi-Fi 网络与 iPhone 对话，iPhone 与其他设备对话。这意味着 HomeKit 逻辑必须嵌入设备本身的固件中，未来对系统的任何修改或扩展都意味着更新固件。

互联网时代不应该是这样的。

设备应该连接到云。在云中，服务器可以相互通信。我们可以在没有危险的无线固件更新的情况下修复错误。

需要明确的是，设备之间的非云连接有一席之地。我们曾经运送过一个音乐同步设备，我们需要的低延迟通信需要本地通信。Nest 也为设备间的本地通信提供了 Weave 平台。蓝牙设备无法连接到 Wi-Fi 接入点，因此需要直接与手机通信。

但是当你可以在云中完成时，没有理由要求*在设备级进行*集成。

## 这太疯狂了

对我来说很奇怪，苹果公司能在这方面犯如此大的错误。这就像在一个有电子邮件的世界里，他们要求我们使用传真机。

我的第一个想法是，他们可能想限制设备的数量，以提高平均质量。如果他们让它足够贵，也许只有最好的设备才能通过。

亚马逊在 First Alert 的 [HomeKit 烟雾探测器](https://web.archive.org/web/20221006185144/https://www.amazon.com/Onelink-Carbon-Monoxide-Battery-HomeKit-enabled/dp/B00R9O328M/)上的评论给出了相反的建议。在今天这个时代，通常不是富有的公司制造最好的设备。

也许只是苹果从根本上来说仍然像一家硬件公司一样思考。也就是说，当他们考虑集成时，他们本能地从硬件需求列表开始。

无论他们的目标是什么，最终的结果都是除非苹果改变做法，否则 HomeKit 将会失败。我希望他们会。天知道 Nest 是否需要一个健康的竞争对手。