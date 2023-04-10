# Trusona 为 sales force TechCrunch 开发无密码访问

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/11/trusona-develops-passwordless-access-for-salesforce/>

上周，为了纪念[世界密码日](https://web.archive.org/web/20221127155916/https://www.passwordday.org/)——是的，真的有这么一个东西——我们发表了我 2015 年的一篇文章，名为[杀死密码](https://web.archive.org/web/20221127155916/https://beta.techcrunch.com/2015/09/07/kill-the-password/)，这是我关于与密码相关的无数问题的论文。试图改变身份的公司 Trusona 今天宣布，它将在 Salesforce.com 发布对无密码进入的支持。嘿，这是个开始。

众所周知，密码的麻烦在于，它给用户带来了创建一个好密码并记住它的负担。如果密码的目的是确保只有授权用户才能访问系统，那么正如我们一次又一次地看到的如此多的高调攻击，它并没有真正做到这一点。

Trusona 希望改变这种状况，让用户无需输入任何信息，就能安全地访问应用和服务。它使用 Salesforce 作为概念验证，但它真的可以应用于任何服务，并且随着时间的推移，您可以期待它们会覆盖其他服务。

你首先要在你的 iOS 或 Android 智能手机上下载 Trusona 应用，并设置你的账户。通过输入 6 位 pin 码，或者如果设备允许，使用您的指纹，您可以在应用程序中确保您的身份。当您打开 Salesforce 应用程序而不是输入用户名和密码时，或者如果您像我一样，单击忘记密码链接，您会单击 Trusona 按钮。

一个二维码立即出现在屏幕上。当 Trusona 应用程序打开时，你将手机摄像头对准屏幕，它就会自动拍照。根据我的经验，它根本不需要操作摄像头就能找到代码。Trusona 首席执行官兼公司创始人 Ori Eisen 表示，他们已经设计了即使从奇怪的角度也能捡起代码的体验。

在摄像头拾取代码后，Trusona 应用程序中会出现一个接受按钮。触摸它，您将登录到 Salesforce。

艾森说，如果你直接从移动设备登录你的应用程序，你只需触摸 Trusona 按钮，它就会深度链接到应用程序，并向你发送 Trusona 应用程序的接受按钮。

[https://web.archive.org/web/20221127155916if_/https://www.youtube.com/embed/CDdKjNxVSXg?feature=oembed](https://web.archive.org/web/20221127155916if_/https://www.youtube.com/embed/CDdKjNxVSXg?feature=oembed)

视频

艾森承认二维码方法并不理想，但他说这是一个起点。“假设二维码是不输入用户名或密码的机制之一，”他说。他们需要机器可读的东西，这是一个起点，但该公司正在研究一种更动态的方法，看起来不像二维码。

此外，你不能试图通过第二次使用相同的授权来欺骗系统，因为该应用程序会匿名记录你手机的遥测数据——经度，纬度，加速度计设置等——而且由于这是一组独特的信息，它永远不会重复。如果系统发现有人试图使用相同的设置授权应用程序，它将拒绝该用户。

Trusona 实际上并没有与 Salesforce 合作来创建这个解决方案。它利用了名为 [SAML](https://web.archive.org/web/20221127155916/http://saml.xml.org/) 的开放身份标准，但它正在与 Salesforce 讨论将该解决方案添加到 Salesforce 的应用商店 AppExchange 中。

艾森告诉我，他利用这项技术的目标是让今年成为最后一个世界密码日——因为如果像他公司这样的技术得到广泛应用，它可能会一劳永逸地消灭密码。