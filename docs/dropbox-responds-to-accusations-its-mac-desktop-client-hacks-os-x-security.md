# Dropbox 回应其 Mac 桌面客户端攻击 OS X 安全 TechCrunch 的指控

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/09/09/dropbox-responds-to-accusations-its-mac-desktop-client-hacks-os-x-security/>

Dropbox 对其如何在苹果 macOS 平台上实现其云存储服务的桌面客户端的担忧做出了回应，承认需要做更多工作来沟通集成如何运行及其请求的权限。

“显然，我们需要更好地宣传 Dropbox 的操作系统集成。我们请求许可一次，但是不描述我们正在做什么或者为什么。Dropbox 桌面客户端团队的本·纽豪斯告诉 TechCrunch。

关于 Dropbox 桌面客户端的担忧今天在[黑客新闻](https://web.archive.org/web/20221226212846/https://news.ycombinator.com/item?id=12463338)和[推特](https://web.archive.org/web/20221226212846/https://twitter.com/mrtoto/status/774284926376108032)上流传，此前[最近在苹果帮助博客上的两篇](https://web.archive.org/web/20221226212846/http://applehelpwriter.com/2016/08/29/discovering-how-dropbox-hacks-your-mac/) [帖子](https://web.archive.org/web/20221226212846/http://applehelpwriter.com/2016/07/28/revealing-dropboxs-dirty-little-security-hack/)详细描述了作者所谓的 Dropbox 对 OS X 安全的“攻击”。在一篇 [AppleHelpWriter 帖子](https://web.archive.org/web/20221226212846/http://applehelpwriter.com/2016/08/29/discovering-how-dropbox-hacks-your-mac/)中，Dropbox 被描述为“利用对 tcc 数据库的 sql 攻击来规避苹果的授权政策。”

尽管 Dropbox 创建了一个欺骗对话框来钓鱼用户密码的指控被证明是不正确的，但批评者继续指责其实现了一个官方的 OS X 安全对话框，他们说该对话框似乎旨在误导用户交出他们的管理员密码，以便通过 Mac 的可访问权限列表授予 Dropbox root 访问系统的权限。

在回应关于客户要求的权限范围的批评时，纽豪斯说:“我们只要求我们积极使用的权限——但不幸的是，有些权限不像我们希望的那样细化。

“我们为 Dropbox 徽章(Office 集成)和其他集成(查找窗口和其他 UI 交互)使用可访问性 API。”

“我们在内置 FS APIs 不足的地方使用提升的访问权限。我们一直在与苹果合作，以消除这种依赖，我们应该很快就会有我们需要的东西，”他补充说。

纽豪斯还声称，Dropbox 没有查看或存储 Mac 用户的管理员密码。

“我们不会看到或存储您的管理员密码。你看到的对话框是一个原生的 OS X API(即由苹果公司制造)，”他说。

至于为什么 Dropbox 首先需要管理员权限，他说:“我们在启动时检查并设置权限——目的是确保 Dropbox 正常运行，跨操作系统更新等。其目的绝不是挫败人们或推翻他们的选择。”

它还使用用户通过操作系统对话框授予的权限来编辑 SQLite 配置文件，以将其自身放在可访问性列表中——尽管它肯定没有明确说明这是用户在响应管理员密码提示时授予的权限。

“我们都在努力。我们会在这里做得更好，我们对我们造成的任何愤怒、沮丧或困惑感到抱歉，”他补充道。

然而，该公司利用根访问将自己放在可访问性列表上以获得系统范围的提升特权的理由并没有给一些批评者留下深刻印象。

作为对 Newhouse 声明的回应，一位黑客新闻评论者 riobard 写道:“此时你需要跟进令人信服的技术细节，说明为什么 Dropbox 需要规避以反击指控并重建受损的信任。

“你的回答中列出的需要可访问性 API 的原因相当模糊，特别是对于那些没有微软产品污染他们系统的 Mac 用户。我现在已经把 Dropbox 从我的 Mac 上删除了。除非有合理的解释和补救措施，否则我是不会把它装回去的。”

另一名黑客新闻评论者 kybernetyk 称，纽豪斯关于“粒度权限”的说法是“对‘一网打尽’权限的委婉说法……”

另一位黑客新闻用户 partycoder 补充道:“现在，恶意软件可以针对你的脚本，免费下载你的所有系统软件。”

对于任何不相信 Dropbox 的*操作方式、*和/或担心授予应用 root 访问权限的安全影响的 Mac 客户端用户，AppleHelpWriter 已经详细介绍了从 OS X 的辅助功能首选项[中移除 Dropbox 的过程。](https://web.archive.org/web/20221226212846/http://applehelpwriter.com/2016/07/28/revealing-dropboxs-dirty-little-security-hack/#comment-27348)

*这篇文章更新了更多细节*