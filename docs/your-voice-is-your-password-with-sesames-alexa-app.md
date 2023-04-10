# 使用芝麻的 Alexa 应用程序，您的声音就是您的密码

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/05/08/your-voice-is-your-password-with-sesames-alexa-app/>

# 在芝麻的 Alexa 应用程序中，你的声音就是你的密码

在 Alexa 的内置功能和[技能 API](https://web.archive.org/web/20230304063149/https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit) 之间，你现在可以使用该平台做几乎任何事情。简单的语音命令可以让你做一些事情，如订购披萨，在 Venmo 上给别人汇款，甚至购买另一台 Echo。

但问题是——任何使用你的 Echo 的人都可以在未经你允许的情况下做这些事情，这可能会让你面临欺诈交易。

幸运的是，TC 的 [Disrupt NY Hackathon](https://web.archive.org/web/20230304063149/https://techcrunch.com/event-info/disrupt-ny-2016/disrupt-ny-hackathon-2016/) 的一个团队决定开发 [Sesame](https://web.archive.org/web/20230304063149/http://devpost.com/software/sesame-zhbw0v) ，这是一款 Alexa 技能应用，可以让你在某些任务中添加语音认证。

要使用这项服务，用户需要进入芝麻的网络应用程序，并发出类似“Venmo Joe $10”的语音命令。然后，芝麻通过将用户的声音与预先录制的密码进行匹配来验证用户的声音，并将请求传递给 Alexa 来完成。

但是为什么芝麻需要基于 web 而不是原生在 Alexa 上呢？因为 Alexa 的 API 实际上并不通过语音传递给开发者，只是用户所说内容的文本转录。由于文本转录显然不足以认证你的声音，芝麻必须作为你的声音和 Alexa 之间的中间物。

Sesame 目前的版本允许你在 Venmo 上给朋友汇钱、订购披萨和发送短信，但该团队预计将增加一些功能，比如只允许某些用户在 Spotify 上更改歌曲或在 Postmates 上下单。

除了 Alexa 的技能 API，该团队还使用了 [VoiceIt](https://web.archive.org/web/20230304063149/https://www.voiceit-tech.com/) 来支持他们的语音认证。

这款应用是由 Shanto Goswami、Kunal Batra 和 Ryan Neff 开发的，他们都是在活动中第一次见面。该团队计划打磨 Sesame，并最终将其作为基于 Alexa 的成熟产品发布。