# 苹果新推出的英特尔驱动 MacBook Pros 有一个辅助 ARM 处理器，运行触控 ID 和安全

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/10/28/apples-new-intel-driven-macbooks-have-a-secondary-arm-processor-that-runs-touch-id-and-security/>

# 苹果新推出的英特尔驱动的 MacBook Pros 有一个运行触控 ID 和安全的辅助 ARM 处理器

苹果什么时候会出货搭载 ARM 处理器的 MacBook？自从该公司从头开始设计和制造自己的芯片以来，这个问题一直是该公司观察家们最关心的问题。

这个问题的答案是现在，某种程度上。苹果新的 13 英寸和 15 英寸 MacBook Pro 型号配备了一个触摸杆——该杆和附带的触控 ID 传感器由笔记本电脑核心的英特尔处理器和苹果设计的 T1 芯片驱动。T1 与新款 Series 2 Apple Watch 的 S2 内部的芯片相同。

T1 由 Apple Watch S2 中的处理器和 Secure Enclave 组成。

正如苹果在其主题演讲中指出的那样，负责触控 ID 传感器的安全，但它也执行各种其他任务。它可以保护相机、存储密码的钥匙链和 Touch Bar。

开发者史蒂文·特劳顿-史密斯昨天公布了其中的一些细节。我能够从我的一些来源获得更多关于 T1 的性质和更多功能的细节和扩展。

T1 还将像素发送到 Touch Bar，尽管 MacBook 的主处理器实际上是渲染然后发送的内容。Touch Bar 上的触摸事件完全由 Mac OS X 驱动，这使得它成为第一个利用 Mac OS 触摸支持的组件。

虽然数据传输由主处理器处理，但苹果支付屏幕上的对话框完全由 T1 呈现，以利用安全飞地，这是芯片中为个人信息留出的一部分，就像 iPhones 和 Apple Watch 设备一样。

Touch Bar 本身运行一个精简的修改版 watchOS，可能是因为 T1 需要它来运行、发送数据和渲染图像。

苹果用这种混合配置做的事情很有意思。它没有“切换”到 ARM 芯片，而是选择为一项精确的任务构建定制芯片，并专门为其使用。正如英特尔芯片擅长繁重的多线程提升 OS X 一样，T1 是为触控 ID 的安全性和安全呈现 Apple Pay 对话框的轻量级提升而设计的。

这种专门的芯片方法是我们在 iPhone 中看到的运动协处理器，但它在 MacBooks 上也很有意义，因为专门的任务由专门的工具处理更好。

这个板载 T1 未来还能实现哪些功能，我们拭目以待。我也比以往任何时候都更加确信，一款内置触控 ID 的 ARM 驱动的 IMAC 和 Mac Pros 键盘正在路上，很快就会到来。