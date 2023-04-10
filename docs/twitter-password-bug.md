# 你应该马上更改你的 Twitter 密码 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/05/03/twitter-password-bug/>

# 你应该马上更改你的推特密码

没错，又到了那个时间——换密码的时间。周四，Twitter 透露，一个[漏洞](https://web.archive.org/web/20221025222025/https://blog.twitter.com/official/en_us/topics/company/2018/keeping-your-account-secure.html)导致该平台以未屏蔽的形式存储用户密码。通常，像密码这样的敏感个人数据会以散列形式存储，使用字母和数字的混合来保护密码本身的内容。在这种情况下，听起来 Twitter 公开存储纯文本密码，而没有对内部日志进行任何哈希处理。

Twitter 指出，目前它“没有理由相信密码信息曾经离开 Twitter 的系统”，或者这些未受保护的密码被黑客访问过，但未知的风险仍然存在。该公司建议用户更改密码作为预防措施。

推特上是这么说的:

> 我们通过使用 bcrypt 函数的哈希过程来屏蔽密码，bcrypt 函数用存储在 Twitter 系统中的一组随机数字和字母来替换实际密码。这使得我们的系统可以在不泄露您的密码的情况下验证您的帐户凭证。这是一个行业标准。
> 
> 由于一个错误，密码在完成哈希过程之前被写入内部日志。我们自己发现了这个错误，删除了密码，并正在实施计划来防止这个错误再次发生。

我们已经联系了 Twitter，以获取关于该错误的更多细节以及关于这是如何发生的更多信息。*更新* : Twitter 拒绝提供关于该事件的更多技术细节，但强调称，其认为密码被发现的可能性“极低”，内部调查显示没有违规或其他滥用的迹象。

对于这种规模的公司来说，犯这样一个基本的安全错误是很不寻常的，但这只是用户自己采取密码保护的另一个原因。现在是开始使用[双因素认证](https://web.archive.org/web/20221025222025/https://help.twitter.com/en/managing-your-account/two-factor-authentication)和类似 [LastPass](https://web.archive.org/web/20221025222025/https://lastpass.com/) 或 [1Password](https://web.archive.org/web/20221025222025/https://1password.com/) 的密码管理器来保护你的账户凭证安全的最佳时机，即使你使用的平台无法做到这一点。