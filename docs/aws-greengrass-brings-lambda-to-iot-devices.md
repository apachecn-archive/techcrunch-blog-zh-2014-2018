# AWS Greengrass 为物联网设备带来 Lambda 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/11/30/aws-greengrass-brings-lambda-to-iot-devices/>

亚马逊今天宣布推出 AWS [Greengrass](https://web.archive.org/web/20221210093816/https://aws.amazon.com/greengrass) ，这是一项新服务，将内置于物联网设备中，为它们带来更好、更智能的计算能力。

正如 AWS 首席执行官 Andy Jassy 在今天亚马逊 re:Invent 开发者大会的主题演讲中指出的那样，亚马逊预计，随着企业将其服务器迁移到云中，大多数内部硬件将很快成为物联网设备。不过，通常情况下，这些物联网设备在 CPU 和本地存储方面都相对较低。当然，这也是这些设备如此依赖云的原因。尽管如此，有时您可能希望在设备上或在连接中断时进行计算。

“利用云来补充这些设备的功能很容易，但有些时候你不想往返于云，”Jassy 指出。“我们现在从两家使用 AWS 物联网产品和设备管理的公司那里听到的重复信息是，他们真正想要的是在这些设备上拥有与他们在 AWS 上相同的灵活性和程序模型来进行计算。"

Greengrass 基于亚马逊的“无服务器”计算服务 AWS IoT 和 AWS Lambda。它将允许开发人员编写可以在物联网设备上运行的 Lambda 代码(用 Python 编写)。Greengrass 核心在本地运行这些 Lambda 功能，但也可以与 AWS 云对话，并允许 IT 管理员管理这些设备和在其上运行的代码。

[![dsc06972](img/eff21863c7351eef63b2429d6991d8a7.png)](https://web.archive.org/web/20221210093816/https://beta.techcrunch.com/wp-content/uploads/2016/11/dsc06972.jpg)

该公司在今天的公告中写道:“如果你已经在为小型设备开发嵌入式系统，现在你将能够利用现代的云感知开发工具和工作流。”"你可以在云中编写和测试你的代码，然后在本地部署."

要做到这一切，亚马逊当然需要合作伙伴，尤其是考虑到它并不构建自己的企业物联网设备。其中包括英特尔和高通，以及 Canonical 和亚马逊自己的[安纳普尔纳实验室](https://web.archive.org/web/20221210093816/http://www.annapurnalabs.com/)。设备需要提供至少 128 MB 的内存和运行速度为 1 GHz 或更高的 x86 或 ARM CPU。

这项服务现在处于预览阶段(尽管现在还不清楚你能从哪里得到兼容的设备)。一旦它正式上市，你将可以免费使用最多三台设备一年。之后，对于多达 10，000 台设备，每个 Greengrass 核心的成本为每月 0.16 美元/台设备。

[![](img/172daff189a8bb2b54a013b82a4b767e.png)](https://web.archive.org/web/20221210093816/https://beta.techcrunch.com/tag/aws-reinvent-2016/)