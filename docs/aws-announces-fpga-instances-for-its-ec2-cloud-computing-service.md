# AWS 宣布其 EC2 云计算服务 TechCrunch 的 FPGA 实例

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/11/30/aws-announces-fpga-instances-for-its-ec2-cloud-computing-service/>

亚马逊的 AWS 云计算服务今天宣布，它将推出一种新的[实例类型](https://web.archive.org/web/20221208011331/https://aws.amazon.com/blogs/aws/developer-preview-ec2-instances-f1-with-programmable-hardware/) (F1)，采用现场可编程门阵列(FPGAs)。FPGAs 的承诺是，它们本质上是可以动态重新编程并针对特定应用进行调整的芯片，使它们比传统的 CPU/GPU 组合更快。

这些[新实例](https://web.archive.org/web/20221208011331/https://aws.amazon.com/ec2/instance-types/f1/)将于今天在 AWS 美国东部地区预览，并将于今年晚些时候全面上市。遗憾的是，该公司尚未宣布这些新实例的定价。

虽然它们仍然远离主流，但 FPGAs 最近变得[更实惠](https://web.archive.org/web/20221208011331/https://www.adafruit.com/categories/69?gclid=Cj0KEQiA6_TBBRDInaPjhcelt5oBEiQApPeTF99832xdo0RiZnppi5mHBTCdvnuVyEHcOlFhTTw_EnYaAo118P8HAQ)且易于编程，这意味着它们也慢慢开始找到进入更多服务的途径。让它们在云中随时可用可能意味着更多的开发人员将开始尝试它们。

AWS 首席执行官安迪·杰西(Andy Jassy)说:“我们总是试图把我们自己可以使用的东西拿出来，并让它对你公开。

这些新的 F1 实例可能会用于高清和 4K 视频处理(而不是 GPU)和成像，以及机器学习。例如，微软在 FPGAs 上投入了全部资金来构建其人工智能服务的后端(而谷歌决定采取更昂贵的路线来构建自己的专用芯片)。由于这些芯片的可重编程性，在应用程序内切换上下文也很容易，因此您可以在某个点处理原始图像，然后重新配置 FPGA 运行深度学习模型，在几毫秒内分析该图像。

AWS 合作测试新 F1 实例的公司之一是 [NGCodec](https://web.archive.org/web/20221208011331/http://ngcodec.com/) 。该公司在短短四周内就将其用于 VR/AR 处理的 RealityCodec 带到了这些新实例中。理想情况下，这可以让开发人员在云中而不是在设备上运行 VR 或 AR 头戴显示器所需的复杂视频处理。正如 NGCodec 创始人 Oliver Gunasekara 告诉我的那样，在 Codec 用例中，FPGAs 比 GPU 有优势，因为编码涉及许多决策，而 GPU 通常不得不将这些决策交给 CPU。Gunasekara 指出，在这种情况下，FPGAs 的能效要高得多。

亚马逊正在使用 Xilinx 的芯片，Xilinx 是最后一家主要的独立 FPGA 制造商。以下是这些新实例的规格:

*   Xilinx UltraScale+ VU9P 采用 16 纳米工艺制造。
*   288 位宽总线上的 64 GiB ECC 保护内存(四个 DDR4 通道)。
*   CPU 的专用 PCIe x16 接口。
*   大约 250 万个逻辑元件。
*   大约 6，800 个数字信号处理(DSP)引擎。
*   用于调试的虚拟 JTAG 接口。

然而，FPGAs 编程仍然很难，而且看起来亚马逊自己也不会发布任何工具来简化编程。不过，将会有一个开发工具包，以及一个机器映像，开发人员可以用它来开始使用这些新实例。

正如 NGCodec 的 Gunasekara 所指出的，Xilinx 本身也发布了一些工具，现在可以更容易地使用更常见的语言，如 C 和 C++来编写 FPGAs(这就是该公司用来设计其 F1 实例的解码器)。

【T2![](img/b289f716150b02b631342faeeec06063.png)