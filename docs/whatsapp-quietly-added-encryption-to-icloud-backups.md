# WhatsApp 悄悄给 iCloud 备份添加了加密技术 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/08/whatsapp-quietly-added-encryption-to-icloud-backups/>

WhatsApp 已经悄悄地为其消息服务的用户增强了 iCloud 备份功能的安全性——这可能会填补一个漏洞，该漏洞可能会使原本端到端加密的消息变得可以以可读的形式访问。比如通过苹果公司的传票，苹果公司持有 iCloud 的加密密钥，或者通过黑客以其他方式获得 WhatsApp 用户 iCloud 账户的访问权限。

据福布斯报道，这家脸书巨头在 2016 年末为 WhatsApp iCloud 备份添加了加密功能，尽管它表示，上周一家提供移动和云黑客工具的第三方公司声称能够绕过安全措施后，这一事实才浮出水面。

有问题的公司 Oxygen Forensics 告诉福布斯，其变通办法只适用于特定的场景，即它可以访问 WhatsApp 用来发送验证码的同一手机号码的 SIM 卡，以生成 iCloud 备份的加密密钥。

WhatsApp 发言人证实，iCloud 备份现在正在加密，他告诉福布斯:“当用户通过 WhatsApp 备份他们的聊天记录到 iCloud 时，备份文件会加密发送。”

取证工具显然被用来下载备份到 iCloud 的加密 WhatsApp 数据。然后，使用相关的 SIM，Oxygen Forensics 表示，它可以通过再次通过验证过程来生成用于解密数据的加密密钥。

《福布斯》建议，例如，警方可以使用这种方法，因为他们的 WhatsApp 账户已经被删除，但 iCloud 备份尚未被清除。

我们已经向 WhatsApp 提出了问题，并将根据任何回复更新这个故事。

对加密的政治压力似乎再次升温。本月早些时候，联邦调查局局长詹姆斯·科米在向参议院监督委员会[提供证据时透露，尽管拥有访问数据的法律授权，但该机构在本财年上半年无法访问 3000 多部移动设备的内容。](https://web.archive.org/web/20221207150926/https://beta.techcrunch.com/2017/05/03/fbi-director-comey-backs-new-feinstein-push-for-decrypt-bill/)

去年，美国联邦调查局卷入了一场与苹果公司的高调斗争，当时它诉诸法庭，试图迫使该公司削弱其安全系统，以帮助调查人员获得锁定的 iPhone。苹果公司拒绝了，最终美国联邦调查局付钱给一家第三方公司来入侵该设备。但该局似乎急于推动立法取缔端到端加密(即服务提供商自己不持有加密密钥)。

在上周的听证会上，科米抱怨称，侵入高度加密的设备和服务的逐案方法不具规模，并支持参议员黛安娜·范斯坦的新呼吁，即立法要求公司在获得授权后解密数据——这为美国又一轮加密战争创造了条件。

WhatsApp 一直处于主流应用用户更容易获得端到端加密的前沿，于 2016 年 4 月完成了该技术在其平台和所有应用中的首次展示。它还抵制法律强制其交出用户数据的尝试——例如在巴西，它的服务已经被[屏蔽](https://web.archive.org/web/20221207150926/https://beta.techcrunch.com/2016/05/02/brazil-orders-cell-phone-carriers-to-block-whatsapp-for-72-hours/)多次，作为对其未能向警方提供解密数据的惩罚。该公司坚称，它不能交出自己没有掌握的信息。

给 iCloud 备份添加加密功能似乎会强化 WhatsApp 的立场，即用户隐私是数据安全的必要条件。尽管如此，关于它是如何在这里实现安全层的，还有一些警告。不启用 WhatsApp iCloud 备份是避免云存储漏洞的更完美的解决方案，尽管从用户的角度来看这可能不方便。