# 黑客组织设法在任天堂 Switch TechCrunch 上运行 Linux

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/02/09/hacker-group-manages-to-run-linux-on-a-nintendo-switch/?ncid=rss&sr_share=googleplus&%3Fncid=sfgplus%0A>

# 黑客组织设法在任天堂 Switch 上运行 Linux

黑客组织 [fail0verflow](https://web.archive.org/web/20230126235610/https://fail0verflow.com/blog/) 分享了一张任天堂 Switch 运行 Linux 发行版 Debian 的照片(通过[任天堂生活](https://web.archive.org/web/20230126235610/http://www.nintendolife.com/news/2018/02/hackers_get_linux_running_on_switch_and_claim_nintendo_cant_patch_the_exploit))。该组织声称任天堂无法用未来的固件补丁修复漏洞。

据 fail0verflow 报道，Nvidia 的 Tegra X1 片上系统中的[引导 ROM](https://web.archive.org/web/20230126235610/https://en.wikipedia.org/wiki/Booting) 存在缺陷。当您的控制台启动时，它读取并执行一段存储在只读存储器(因此得名 ROM)中的代码。此代码包含关于引导过程的说明。

这意味着启动 ROM 在 Nvidia 生产时就存储在芯片上，之后就不能以任何方式更改了。即使任天堂发布了软件更新，这个软件更新也不会影响引导 ROM。由于控制台在按下电源按钮后会立即加载启动 ROM，因此无法绕过它。

解决这个问题的唯一方法是制造新的 Nvidia Tegra X1 芯片。因此，任天堂有可能要求英伟达解决这个问题，以便新的游戏机没有这个漏洞。

fail0verflow 还说不需要安装修改芯片来绕过引导 ROM。在照片上，看起来他们在设备的右侧插上了什么东西，那里应该是正确的 Joy-Con。

如果 fail0verflow 决定分享这一漏洞，它可能会为自制软件和盗版游戏带来许多可能性。这可能会给任天堂带来一些财务影响。