# 安全研究人员在 WhatsApp 群聊中标记邀请错误

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/01/10/security-researchers-flag-invite-bug-in-whatsapp-group-chats/>

安全研究人员透露了 WhatsApp 安全漏洞的细节，该漏洞可能被用来破坏消息平台上加密群聊的保密性。

由于攻击者需要访问 WhatsApp 服务器才能将自己插入群组对话，因此与该漏洞相关的风险有限。

也就是说， [WhatsApp 在使用](https://web.archive.org/web/20230330033952/https://techcrunch.com/2017/10/04/uk-gives-whatsapp-another-spanking-over-e2e-crypto/)[端到端加密](https://web.archive.org/web/20230330033952/https://techcrunch.com/2017/06/05/we-want-to-limit-use-of-e2e-encryption-confirms-uk-minister/)方面确实继续面临来自政府的压力。因此，任何漏洞，甚至可能*理论上*提供一个途径，让该公司被国家实体胁迫与他们的代理人合作，以提供一定程度的访问加密对话的机会，都值得强调。

《连线》报道称，今天在瑞士苏黎世举行的真实世界加密安全会议上，德国波鸿鲁尔大学的一组研究人员详细介绍了加密缺陷，这些缺陷也影响了 Signal 和 Threema 消息应用程序——尽管程度较轻。

关于 WhatsApp，研究人员表示，任何控制 WhatsApp 服务器的人都可以在未经群组管理员许可的情况下，将新参与者插入一个私人群组。

这次攻击显然利用了 WhatsApp 处理群聊的一个缺陷——虽然只有一个群的管理员才能邀请新成员，但该平台不会对其自己的服务器无法欺骗的邀请使用任何认证机制。

一旦能够访问 WhatsApp 服务器的攻击者在一个群组中添加了一名新成员，每个参与者的手机都会自动与该新成员共享密钥——让他们能够完全访问任何未来的消息。(尽管在他们加入群组之前发送的消息仍然不可读。)

虽然聊天中的每个人都会被通知有新成员加入，但很可能由管理员来通知并发出欺骗性邀请(因为他们是能够创建邀请链接的用户)。

研究人员还建议，能够访问 WhatsApp 服务器的攻击者可以选择性地阻止群中的任何消息——关闭群参与者提问的能力，或者提供关于入侵者的警告。

联系到 WhatsApp 的发言人进行评论，他证实了安全研究人员的发现，但表示认为风险有限，因为没有人可以秘密加入 WhatsApp 的群聊——这意味着用户可以一直一对一地聊天，以确认对出现在他们群中的未知成员的任何怀疑。

“我们已经仔细研究了这个问题，”一位发言人告诉我们。“当有新成员加入 WhatsApp 群组时，现有成员会收到通知。我们开发了 WhatsApp，这样群发消息就不会发送给隐藏的用户。用户的隐私和安全对 WhatsApp 来说非常重要。这就是为什么我们收集的信息很少，所有在 WhatsApp 上发送的消息都是端到端加密的。”

安全研究人员团队去年 7 月向 WhatsApp 披露了这一缺陷，他们建议该公司可以通过为新的群邀请添加认证机制来解决这一问题，该机制使用只有管理员拥有的秘密密钥来签署这些邀请。

这种增加的身份验证层可能会使 WhatsApp 无法提供允许人们快速向群中添加新成员的群邀请链接——这解释了为什么该公司不愿意改变其现有的系统，尽管存在明显的风险。

它还指出，WhatsApp 用户可以通过点击“群组信息”来查看群组成员，并可以验证单个成员的安全代码以增加安全性。

对于使用与 WhatsApp 相同的底层加密协议的 Signal messaging 应用程序，安全研究人员发现该应用程序包含相同的群聊漏洞，但攻击者不仅必须控制相关的 Signal 服务器，还必须知道聊天的群 ID 号(这些 ID 基本上是不可访问的)，从而进一步缓解了这一漏洞。

运行和维护 Signal 的非营利组织 Open Whisper Systems 显然也在重新设计 Signal 处理群组消息的方式。

第三个加密信息应用程序 Threema 也被研究人员发现包含一些与群聊有关的小错误，它已经发布了一个修补软件的补丁。

去年[1 月](https://web.archive.org/web/20230330033952/https://techcrunch.com/2017/01/13/encrypted-messaging-platform-whatsapp-denies-backdoor-claim/)与 WhatsApp 平台相关的另一个安全问题在一名安全研究人员展示了强制为离线用户生成新的加密密钥的可能性后[被强调](https://web.archive.org/web/20230330033952/https://techcrunch.com/2017/01/13/encrypted-messaging-platform-whatsapp-denies-backdoor-claim/)——重新引发了关于如何在加密系统中实现密钥验证的辩论。然而，WhatsApp 表示，“重新传输漏洞”是一个有意的设计决策，旨在避免数百万条信息丢失。

它还指出，用户可以选择“显示安全通知”——当联系人的安全代码发生变化时，会向他们提供通知，因此当/如果他们的信息有被中间人拦截的风险时，会发出警报。