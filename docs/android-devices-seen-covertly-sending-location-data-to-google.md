# 安卓设备被发现偷偷向谷歌 发送位置数据

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/11/21/android-devices-seen-covertly-sending-location-data-to-google/>

Quartz 的一项调查显示，即使用户在设备设置中禁用了应用程序的定位服务，安卓设备也会向谷歌发送手机信号塔的位置数据。

Quartz 还表示，即使设备被重置为出厂默认设置，它也观察到位置数据正在被发送。每次进入新手机信号发射塔的范围时，拥有蜂窝数据或 wi-fi 连接的 Android 设备都会向谷歌发送数据，包括没有安装 SIM 卡的设备(这些设备通过 wi-fi 下载位置数据，如果有的话)。

它表示，目前 Android 用户没有办法阻止他们的位置数据被发送到广告目标巨头谷歌——除非从他们的设备中删除 sim 卡并禁用 wi-fi(或者将设备留在法拉第笼内)。

在向谷歌提出这一发现后，Quartz 报告称，公司发言人告诉它，手机信号塔位置数据收集已经持续了 11 个月，手机信号塔地址包含在发送给系统的信息中，该系统用于管理 Android 设备上的推送通知和消息。

该发言人进一步声称，位置数据从未被使用或存储。谷歌补充说，它打算在 11 月底结束这种做法，因为 Quartz 已经向它指出了位置跟踪问题。

谷歌发言人表示:“今年 1 月，我们开始研究使用手机识别码作为额外的信号，以进一步提高信息传递的速度和性能。”“但是，我们从未将 Cell ID 整合到我们的网络同步系统中，因此数据会立即被丢弃，我们将其更新为不再请求 Cell ID。”

不管谷歌尝试收集安卓用户位置信息的原因是什么，这是该公司在没有让人们明确意识到的情况下吸收敏感用户数据的又一个令人不安的例子——更不用说让用户控制选择退出另一次重大的隐私侵犯了。

回到[10 月](https://web.archive.org/web/20230316161016/https://techcrunch.com/2017/10/10/google-home-mini-recorded-24-7-androidpolice/)，例如，许多 Google Home Mini 设备出现故障，并持续在主人家中的背景中录制音频，而不是只在使用特定触发词时才被唤醒。

在这一混乱引起媒体关注后，谷歌表示将[移除设备上的 touch top 功能](https://web.archive.org/web/20230316161016/https://techcrunch.com/2017/10/11/citing-a-few-malfunctions-google-nukes-touch-function-from-home-mini/)——指责硬件故障引发了对用户家庭活动的近乎连续的记录。因为它现在指责 Android 秘密收集位置数据的工程实验。

位置数据是高度敏感的个人数据，从中可以推断出一个人的生活和生活方式，特别是考虑到移动设备的规则是无论用户去哪里都要陪伴用户。虽然手机信号发射塔的位置数据不一定非常精确，但多个手机信号发射塔的三角测量可以用来计算更精确的位置。

因此，即使 Android 操作系统知道用户的手机信号塔位置可以提高消息速度和性能，谷歌至少应该要求人们选择加入这一位置跟踪增强功能，并/或为他们提供一种选择退出的方式。

谷歌的[隐私政策](https://web.archive.org/web/20230316161016/https://www.google.com/policies/privacy/)确实包括以下关于“位置信息”的部分(如下)，该部分声明“谷歌服务”的用户可能会收集他们的位置数据，包括手机信号塔数据——尽管谷歌使用的链接示例指的是特定的谷歌应用程序，如谷歌地图，而不是安卓操作系统本身；虽然 wi-fi 接入点和手机信号发射塔的链接示例仅涉及为启用了谷歌位置服务的用户收集位置数据(不是永久收集，因为你使用的是 Android 操作系统):

> 当您使用谷歌服务时，我们[可能会收集和处理有关您实际位置的信息](https://web.archive.org/web/20230316161016/https://www.google.com/policies/privacy/example/may-collect-and-process-information.html)。我们使用各种技术来确定位置，包括 IP 地址、GPS、[和其他传感器](https://web.archive.org/web/20230316161016/https://www.google.com/policies/privacy/example/sensors.html)，例如，这些传感器可以为谷歌提供附近设备的信息、 [Wi-Fi 接入点和手机信号发射塔](https://web.archive.org/web/20230316161016/https://www.google.com/policies/privacy/example/wifi-access-points-and-cell-towers.html)。

根据 Quartz 的发现，位置追踪似乎并不局限于特定的安卓手机或平板电脑。报告称，谷歌显然在收集所有现代安卓设备的手机信号塔数据。

它还援引一位知情人士的话说，在 2017 年初谷歌拥有的、默认情况下在安卓手机上运行的 [Firebase 云消息](https://web.archive.org/web/20230316161016/https://firebase.google.com/docs/cloud-messaging/)服务发生变化后，手机信号塔地址被发送给了谷歌。

虽然这是一个值得注意的例子，Android 平台控制器谷歌本身显然被发现通过操作系统秘密跟踪用户的位置，但这次[去年](https://web.archive.org/web/20230316161016/https://techcrunch.com/2016/11/15/budget-us-android-smartphones-found-secretly-sending-personal-data-to-china/)在美国销售的一系列廉价 Android 智能手机被发现秘密向位于中国的第三方公司发送个人数据——包括用户的位置信息。

尽管在这种情况下，罪魁祸首是预装在设备上的商业固件，而不是 Android 操作系统本身，就像这里一样。