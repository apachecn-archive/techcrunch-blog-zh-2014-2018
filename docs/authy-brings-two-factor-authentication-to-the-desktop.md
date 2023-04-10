# Authy 为桌面带来双重身份认证

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/04/28/authy-brings-two-factor-authentication-to-the-desktop/>

当你使用双因素认证时，你可能会从手机应用程序中获得第二个因素，如谷歌[认证器](https://web.archive.org/web/20230316161016/https://support.google.com/accounts/answer/1066447?hl=en)或[认证器](https://web.archive.org/web/20230316161016/http://authy.com/)。这是有意义的，因为你想确保没有人可以访问你的电脑，也可以访问为你提供访问你的私人账户的第二个密钥的应用程序。

[Authy](https://web.archive.org/web/20230316161016/http://authy.com/) 今天颠覆了这个想法，推出了一款桌面应用，用于其双因素认证服务。Authy for Desktop [现在可以作为 Chrome 应用在这里](https://web.archive.org/web/20230316161016/https://chrome.google.com/webstore/detail/authy/gaedmjdfmmahhbjefcbgaolhhanlaolb)使用。虽然它使用 Chrome 的应用程序框架，但它是一个完全独立的应用程序，你不需要运行 Chrome 来使用它。这种方法允许同一个应用程序在 Windows、Mac 和 Linux 上运行。

正如该公司创始人兼首席执行官丹尼尔·帕拉西奥(Daniel Palacio)上周告诉我的那样，能够从台式机和笔记本电脑中获得第二个因素有助于实现更加无缝的用户体验。你可以从桌面应用程序中复制并粘贴代码，而不是键入代码。对于那些没有智能手机的用户来说，这也提供了一种更简单的替代方式来代替通常的短信服务，如 Authy 利用发送他们的代码。

通过切换到桌面应用程序，只有当你登录到另一台不受你控制的电脑时，你的手机才变得重要。

但是，这不是违背了双因素应用程序的目的吗？authy——不出所料——声称不会。该公司今天在[的一篇博客文章中写道:“无论‘你拥有的’第二认证因子是来自你的手机、平板电脑，还是直接来自你笔记本电脑中的桌面应用程序，双重认证仍然有效。“真正重要的是，这是只有你才能拥有的东西。”](https://web.archive.org/web/20230316161016/http://blog.authy.com/authy-for-pc)

![chrome-master-pwd](img/7f8f0904effdd76b6df5bec474e4db5b.png) Palacio 还指出，虽然大多数人没有意识到这一点，但 RSA Security——企业公司领先的双因素身份认证服务之一——早就提供了一个[桌面应用程序](https://web.archive.org/web/20230316161016/http://www.emc.com/security/rsa-securid/rsa-securid-software-authenticators/ms-windows.htm)。

该公司称，双因素身份认证也从未被设计用来防止设备被盗。为了在你的电脑被盗的不幸情况下保护你的账户，Authy 允许你用一个主密码加密你所有的本地账户。由于 Authy 的[最近推出了](https://web.archive.org/web/20230316161016/https://techcrunch.com/2013/11/21/authy-goes-where-no-two-factor-authentication-system-has-gone-before-to-multiple-devices/)功能，可以使用多种设备获取您的第二个因素，您也可以轻松地停用您的令牌，以防您的笔记本电脑被盗。

该公司还认为，虽然可能有恶意软件安装在你的本地机器上，可能会窃取你的双因素令牌，但这是一个问题，无论你使用两个独立的设备还是只有一个。最后，您的会话 id 通常会存储在本地会话 cookie 中，告诉给定的站点该会话确实已经过身份验证。如果应用程序可以访问它，那么第二个因素来自哪里就无关紧要了。

![chrome-phishing](img/bcb71e59903c17375f681ac72ad02dec.png)

安装了 Authy for Desktop 应用程序和该公司的新 Chrome 扩展的用户还将获得 Authy 的钓鱼检测的额外好处。这个扩展让服务可以访问你所有的活动标签，然后根据一个官方网址的白名单来验证这些标签。每当用户试图将访问令牌复制到不在白名单上的站点时，该服务都会抛出错误。

总的来说，帕拉西奥认为 Authy for Desktop“可能是我们做过的最好的应用。”他还告诉我，该公司也一直在尝试使用你的手机本身作为第二个因素。然而，蓝牙 LE 在智能手机中的低渗透率仍然是一个问题。

Authy 目前保护着大约 100 万个账户，有超过 60 万人定期使用。