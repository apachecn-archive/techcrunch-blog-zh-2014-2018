# 人们用“杀手符号”吸引 iPhone 用户，使他们的应用崩溃

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/16/iphone-bug-telugu-unicode-ios-mac-text-bomb/>

惊喜！互联网上各种各样的怪人已经将我们昨天报道的基于 Unicode 的漏洞武器化，使运行在 iPhone 或 Mac 上的应用程序崩溃。结果介于旧的 Alt + F4 技巧和脚本小子特技之间，从令人讨厌到使设备无法使用，取决于巨魔的坚韧程度。

该漏洞导致许多 iOS 和 Mac 应用程序在南印度语泰卢固语中渲染两个字符时崩溃。虽然任何人都可以避免看到这些符号，但当有人恶意发送这些符号或将它们直接发送到接收通知的设备时，问题就出现了。

在过去的一天里，许多 Twitter 用户已经开始在 Twitter 上发布这些符号，比如“阅读这篇文章立即注销”和“转发这篇文章让任何使用苹果设备的人崩溃”，不过幸运的是，他们中的大多数人没有多少粉丝。不过，如果这个符号出现在你的@回复中，或者出现在某个喜欢你的推文的人的手柄中，那么你打开的任何应用程序的游戏都结束了(主板作家约瑟夫·考克斯[吃了苦头才知道这一点](https://web.archive.org/web/20230324125434/https://motherboard.vice.com/en_us/article/bj573w/iphone-twitter-text-bomb-crash-ios))。根据我们的观察，让一个应用程序重新工作的唯一方法是从头开始重新安装——这是一个耗时的过程，尤其是如果一个巨魔再次让它崩溃的话。

正如在推特上捕捉到的，一名安全研究员[在他的优步手柄](https://web.archive.org/web/20230324125434/https://twitter.com/_MG_/status/964261495423954944/photo/1?ref_src=twsrc%5Etfw&ref_url=https%3A%2F%2Fbeta.techcrunch.com%2Fwp-admin%2Fpost.php%3Fpost%3D1599542%26action%3Dedit%26recrawl%3Dtrue%26code%3D200%26response_body%3DQueued)上添加了一个符号作为实验。“我怀疑一个死机的手机意味着你被转到下一个司机那里……那个司机也死机了。就像优步路由蠕虫，”他写道。我们联系了优步，看看他们是否意识到了这个问题，并会在我们得到回复时更新。

![](img/6450194f310aa895ab202ed746a2926e.png)

目前，大部分的钓鱼似乎是在 Twitter 上。在脸书和 Reddit 上的搜索都没有发现太多泰卢固语的痕迹，因此这些平台似乎已经采取措施来限制扼杀 iPhone 的 Unicode 符号的影响。

与此同时，Mozilla 工程师马尼什·戈雷戈卡尔(Manish Goregaokar)的博客文章指出，Unicode 错误的范围可能比我们所知的两种符号更广。“……根据一些实验，这种错误似乎发生在任何一对带元音的泰卢固语辅音上，只要元音不是ై (ai)，”他写道。他目前的发现是:

> 所以，最终，导致崩溃的所有情况是:
> 
> 梵文、孟加拉文和泰卢固文中的任何序列<consonant1 virama="" consonant2="" zwnj="" vowel="">，其中:</consonant1>
> 
> 辅音 2 是后缀连接，即र、র、য和所有泰卢固语辅音
> 如果辅音 2 是र或র，辅音 1 不是同一个字母(或变体，如ৰ)
> 元音不是ై或ৌ

TechCrunch 已经联系了 Twitter、脸书和 Reddit，看看这些平台是如何处理这个漏洞的，当这个漏洞在一个开放的社交网络上爆发时，破坏性尤其大。我们也与苹果公司取得了联系，他们已经确认即将推出“点更新”修复，但拒绝确认是否会是 iOS 11.2.6。苹果指出，该漏洞已在 iOS、tvOS、macOS 和 watchOS 的当前测试版中得到修复。