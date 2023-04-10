# 微软发布其新的端到端物联网解决方案 Azure Sphere

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/04/16/microsoft-built-its-own-custom-linux-kernel-for-its-new-iot-service/>

在旧金山的一场小型新闻发布会上，微软今天[宣布](https://web.archive.org/web/20230406224646/https://azure.microsoft.com/en-us/blog/introducing-microsoft-azure-sphere-secure-and-power-the-intelligent-edge/)推出一款安全的端到端物联网产品，该产品专注于基于微控制器的设备——这种设备使用微小且相对低功率的微控制器(MCU)来实现基本控制或连接功能。通常情况下，这类设备可能是任何东西，从玩具到家用小工具或工业应用程序，不会经常更新，因此安全性经常受到影响。

在 [Azure Sphere](https://web.archive.org/web/20230406224646/https://www.microsoft.com/en-us/azure-sphere/) 的核心是一类新的认证 MCU。正如微软总裁兼首席法律官布拉德·史密斯在今天的公告中强调的那样，微软将免费授权这些新的 Azure Sphere 芯片，希望借此启动 Azure Sphere 生态系统。

因为很难保护一个无法更新或获取遥测数据的设备，所以这些设备将内置连接也就不足为奇了。通过这种连接，这些设备也可以连接到云中的 Azure Sphere 安全服务。

现在，你可能认为这些设备将运行 Windows，但你错了。微软有史以来第一次推出定制的 Linux 内核和发行版:Azure Sphere OS。这是对当今 MCU 经常使用的实时操作系统的更新。

为什么要用 Linux？“通过 Azure Sphere，微软正在解决一个全新的物联网设备类别，即 MCU，”微软 Windows 企业和安全合作伙伴总监罗布·莱弗茨在活动中告诉我。“Windows IoT 运行在微处理器单元(MPU)上，其能力至少是 MCU 的 100 倍。Azure Sphere 物联网操作系统中使用的微软安全 Linux 内核在 OSS 许可下共享，因此芯片合作伙伴可以快速实现新的芯片创新。”这些合作伙伴也非常乐意采用开源版本并将其集成到他们的产品中。

为了启动这一进程，[联发科](https://web.archive.org/web/20230406224646/https://www.mediatek.com/news-events/press-releases/mediatek-collaborates-with-microsoft-to-advance-innovation-and-security-for-the-intelligent-edge)正在生产[第一套](https://web.archive.org/web/20230406224646/https://www.mediatek.com/products/azureSphere/mt3620)这种新型微处理器。这些是低功耗、单核 ARM-A7 系统，运行速度为 500MHz，包括 WiFi 连接和许多其他 I/O 选项。

就开放生态系统而言，史密斯还强调，这些设备可以与运行在任何其他云上的服务一起使用，无论是 AWS 还是阿里云。

有趣的是，亚马逊的 AWS 部门在去年的 re:Invent 大会上宣布了一个有点类似的项目。这些大型云提供商对 MCU 感兴趣可能并不奇怪，因为尽管设备本身没有绑定到任何云，但从它们那里获得全部价值的唯一方式是与云服务相结合，无论是用于认证新设备、更新操作系统还是管理在其上运行的软件。