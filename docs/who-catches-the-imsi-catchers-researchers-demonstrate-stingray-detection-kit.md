# 谁抓 IMSI 捕手？研究人员展示魟鱼检测工具

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/06/02/who-catches-the-imsi-catchers-researchers-demonstrate-stingray-detection-kit/>

IMSI 捕捉器，用来欺骗信号塔和拦截通信的设备,是执法部门最讨厌的公开秘密之一。严格的保密协议阻止它们被承认存在，更不用说被使用了——但是研究人员认为他们已经找到了一种发现可疑信号窃取者的方法。

这种设备，俗称黄貂鱼，根据一种常见的模型命名，通过发出信号来工作，就像手机信号塔一样；手机通过假塔连接、识别自己并发送短信和电话等信息，创造了一种移动窃听。批评者认为，无辜者的数据陷入了这张罗网，但由于提供这些设备的公司发出了禁言令，执法部门一直不太配合。

我们需要一种独立的方法来识别野外的 IMSI 捕手。这就是华盛顿大学的研究人员彼得·内伊和伊恩·史密斯[试图用 SeaGlass](https://web.archive.org/web/20230306050623/https://seaglass.cs.washington.edu/) 创造的东西。

“到目前为止，世界各地 IMSI 捕手的使用一直笼罩在神秘之中，这种具体信息的缺乏是知情公众讨论的障碍，”[在 UW 新闻发布会上解释道。“拥有关于基站模拟器的额外、独立和可信的信息来源，对于了解如何以及如何负责任地使用它们至关重要。”](https://web.archive.org/web/20230306050623/http://www.washington.edu/news/2017/06/02/catching-the-imsi-catchers-seaglass-brings-transparency-to-cell-phone-surveillance/)

[![](img/52d5611fe3a463c688e3a90a4e732007.png)](https://web.archive.org/web/20230306050623/https://techcrunch.com/wp-content/uploads/2017/06/rig_labeled.png)

该团队组装了一种超级动力的驾驶设置，使用“诱饵电话”，GSM 调制解调器，GPS 单元，Wi-Fi 热点和其他无线小玩意包装在一个盒子里。这些设备监控并记录它们遇到的无线信号。为了覆盖尽可能多的区域，西雅图和密尔沃基的拼车司机在 15 辆车上安装了盒子。

[![](img/db07417b12aaa42534241bd477fb591d.png)](https://web.archive.org/web/20230306050623/https://techcrunch.com/wp-content/uploads/2017/06/seaglass-baseline-gif-2.gif)

随着它的增长而显示的基线图；红色信号更强、更可靠

在两个月的时间里，这些工具包收集了无线活动的基线，包括已知的发射塔、私人信号等等。但是筛选数据揭示了一些可疑的异常信号。

例如，一个信号源在两个月内改变了六次传输频率——这与 96%被检测到的信号源不同。其中五个频率只能在离大楼 1500 英尺的范围内被探测到。

人们可能会把它记为一种测试或纳米细胞，除非这个特殊的来源恰好位于国土安全部管理的移民服务大楼内或附近。那会是一条黄貂鱼吗？它会瞄准新移民吗？数据与假设一致，但是需要更多的数据来确定。

[![](img/3ccf8e46ac4fd0dcd75dc84f22d44c71.png)](https://web.archive.org/web/20230306050623/https://techcrunch.com/wp-content/uploads/2017/06/customs_building.png)

被讨论的建筑，用菱形表示，产生了许多正常的信号(绿色)，但是在近距离产生了可疑的信号(其他颜色)

“我们要谨慎对待我们的结论，”史密斯提醒道。“我们确实在某些位置发现了奇怪而有趣的模式，这与我们预计从蜂窝基站模拟器中看到的模式相匹配，但这是我们从初步试点研究中能说的最多的。”

至少它也为倡导者和记者提供了一些工作素材。去年，在试图发现西雅图警方是否使用黄貂鱼时，我发现自己缺乏尖锐的问题可问:尽管我得到了明确的“不”，而不是拒绝，但最好有一些具体的想法，如地点或行动。我可以问问 DHS 关于上面提到的可疑信号。

不幸的是，该团队无法得到一个真正的 IMSI 捕手来证明这些发现——这些设备被他们的管理员小心翼翼地保护着，关于它们的信息实际上只能通过[泄露的文件](https://web.archive.org/web/20230306050623/https://theintercept.com/surveillance-catalogue/stingray-iii/)和偶尔遗漏的编辑来获得。史密斯在一封电子邮件中告诉我，他们确实根据他们对这些东西如何工作的了解，推出了他们自己的类似黄貂鱼的设备。

[![](img/4cf51096bd2cdf05c967a12be8f0d7e3.png)](https://web.archive.org/web/20230306050623/https://techcrunch.com/wp-content/uploads/2017/06/peter_ian_seaglass.jpg)

研究人员彼得·内伊(左)和伊恩·史密斯

检测套件包含价值约 500 美元的部件，[，所有这些都在描述工作的文件中有详细说明](https://web.archive.org/web/20230306050623/https://seaglass-web.s3.amazonaws.com/SeaGlass___PETS_2017.pdf)。不过，史密斯认为成本可以随着规模的扩大而降低。

“我们渴望将此推广到社区，并找到能够众包更多数据收集的合作伙伴，并开始以有意义的方式连接这些点，”他说。

透明度倡导者当然希望有一个这样的工作系统，尽管也必须指出，犯罪分子也会发现它很有用。但是任何工具都是如此，包括 IMSI 捕手。

你可以找到更多关于这个工具的信息，或者探索团队在 SeaGlass 站点收集的数据[。](https://web.archive.org/web/20230306050623/https://seaglass.cs.washington.edu/)