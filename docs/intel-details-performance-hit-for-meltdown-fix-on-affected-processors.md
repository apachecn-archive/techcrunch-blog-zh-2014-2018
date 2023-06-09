# 英特尔详细介绍受影响处理器的性能崩溃修复技术 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/01/11/intel-details-performance-hit-for-meltdown-fix-on-affected-processors/>

现在 [Meltdown 和 Spectre](https://web.archive.org/web/20221207215223/https://beta.techcrunch.com/2018/01/03/kernel-panic-what-are-meltdown-and-spectre-the-bugs-affecting-nearly-every-computer-and-device/) cats 已经公开了，补丁到处都在发布，人们的主要问题是:这会影响我的日常工作吗？英特尔的最新性能指标表明，是的，它可能会，但不会太多——如果你像我一样，有一个更老的处理器，就更是如此。

英特尔的 Navin Shenoy [发布了内部完成的几项基准测试的结果](https://web.archive.org/web/20221207215223/https://newsroom.intel.com/editorials/intel-security-issue-update-initial-performance-data-results-client-systems/)，谷歌研究人员披露的根深蒂固的处理器问题对性能的影响对于现代芯片来说是幸运的小。

去年年底推出的最新 Kaby Lake 处理器在 SYSmark14SE 中的性能损失通常不到 5%，甚至根本没有。(误差幅度规定为+/-3%。)

但对这些 CPU 来说，实际上大多数其他 CPU 也是如此，最大的打击在于“响应能力”，根据基准应用程序的创建者，这包括“应用程序启动、文件启动、多标签网页浏览、多任务处理、文件复制、照片处理、文件加密+压缩和后台应用程序安装。”所以，大部分人需要做的事情。

游戏性能似乎基本不受影响，大多数 GPU 受到的影响更有限，或者根本不受攻击及其缓解措施的影响，游戏玩家可能可以高枕无忧了。

那些采用旧处理器的处理器可能会看到真正的放缓，例如，2015 年年中发布的第六代酷睿 i7 6700K。它的性能损失接近 10 %,在 Windows 10 上，响应速度下降了 31%。自然，这就是我的确切设置——很可能是当时购买这些非常受欢迎的芯片的许多用户的设置。

英特尔分享的这张图表显示了原始数据，即芯片未修补性能的百分比。

[![](img/f75f1936f79f6b034b1c1a3e2c49e6a7.png)](https://web.archive.org/web/20221207215223/https://beta.techcrunch.com/wp-content/uploads/2018/01/intel-meltdown-performance-chart.png)

图表攻击！

旧的设置可能会受到更深的影响，但我们可以等待结果。这些芯片的真正风险是，它们嵌入在难以修补的嵌入式或难以触及的系统中，从而使它们容易被利用。不过，到目前为止，还没有黑客利用这些漏洞的报道——这并不完全是儿童脚本。

奇怪的是，在一些情况下，性能有所提高，尽管谁知道这是怎么发生的。Shenoy 没有提到这笔意外的横财，尽管它可能很小。

因此，如果你注意到你的电脑在接下来的几周里变慢了，那不仅仅是你，也不是苹果的阴谋——不幸的是，这是修复崩溃的必然结果。