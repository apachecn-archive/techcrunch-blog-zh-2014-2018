# 微软开源 PowerShell，将其引入 Linux 和 OS X 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/08/18/microsoft-open-sources-powershell-brings-it-to-linux-and-os-x/>

微软今天宣布开源 PowerShell 并将其引入 Linux 和 OS X。

PowerShell 是微软为 Windows power 用户提供的命令行 Shell，也是一种用于自动化系统任务的可扩展脚本语言。这与 Linux 上的 Bash 没有什么不同(T2 现在的 Windows T3 也是如此)，但是与 Windows 有着更深的联系。然而，微软正在改变，正如其首席执行官塞特亚·纳德拉倾向于重复的那样，它意识到它现在在一个“多平台、多云、多操作系统的世界”中运营这意味着该公司现在经常做一些仅在几年前还不可思议的事情。将 Linux 子系统构建到 Windows 10 中，并开源其部分核心工具？那现在是意料之中的事。

[![11524380](img/dd08c90e1f6971749d612b5f4ca6a522.png)](https://web.archive.org/web/20230127141259/https://techcrunch.com/wp-content/uploads/2016/08/11524380.png) 正如微软技术研究员、企业云团队首席架构师杰弗里·斯诺弗告诉我的那样，纳德拉基本上告诉公司要与客户交谈，找出他们成功所需的东西，并给予他们。“我们听说客户希望有自己选择的客户端、服务器和云，”斯诺弗告诉我。“我们希望成为客户运行工作负载的首选合作伙伴，帮助他们管理一切符合微软和客户的共同利益。”斯诺弗补充说，通过 PowerShell，微软现在可以为客户提供“他们喜欢的任何客户端上的单一管理堆栈”(当然，假设你喜欢的客户端是 Windows、OS X 和 Linux)。

微软为今天的发布做好了准备，它[开源了它的。NET 框架](https://web.archive.org/web/20230127141259/https://techcrunch.com/2016/06/27/microsofts-open-source-net-and-asp-net-core-hit-1-0/)而制成。NET Core 可用于 Linux 和 OS X。所以这两个团队合作将 PowerShell 带到这些新的平台上。

然而，实际的外壳只是 PowerShell 强大的一部分。微软还将 PowerShell 编辑器服务引入 Linux，这样开发人员就可以在他们的文本编辑器中构建对它的支持(已经提供了对 Visual Studio 代码和 Sublime 的支持)。

[https://web.archive.org/web/20230127141259if_/https://www.youtube.com/embed/2WZwv7TxqZ0?feature=oembed](https://web.archive.org/web/20230127141259if_/https://www.youtube.com/embed/2WZwv7TxqZ0?feature=oembed)

视频

PowerShell 也是高度可扩展的，许多微软合作伙伴，如 VMware——甚至是它的[云竞争对手 AWS](https://web.archive.org/web/20230127141259/https://aws.amazon.com/powershell/) —已经为 PowerShell 构建了微软所谓的 cmdlets，允许你直接从 Shell 或脚本中管理 EC2 实例。

PowerShell 还集成了微软[运营管理套件](https://web.archive.org/web/20230127141259/https://www.microsoft.com/en-us/cloud-platform/operations-management-suite) (OMS)，允许您在几乎任何平台上管理您的应用程序和工作负载，包括 Azure、AWS、谷歌的云平台和内部数据中心部署。

至于将 Bash 引入 Windows 和将 PowerShell 引入 Linux/OS X 之间的区别，斯诺弗指出，Bash 在 Windows 上的重点是让开源开发者能够在 Windows 上工作。

斯诺弗承认，微软仍在学习如何最好地管理这类开源项目，但他的团队已经花了很多时间与合作伙伴讨论如何做到这一点，以及如何使其成功。他还指出，微软计划推出一个社区治理模型，并将从社区中获取代码更改，这些代码更改也可能最终出现在 PowerShell for Windows 中。

Ubuntu、CentOS 和 Red Hat 上的 Linux 用户，以及 OS X 用户现在可以从 [PowerShell GitHub 库](https://web.archive.org/web/20230127141259/https://github.com/PowerShell/PowerShell)下载运行 PowerShell 所需的位。