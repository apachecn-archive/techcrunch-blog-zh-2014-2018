# 人机交流的新典范 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/08/24/the-new-paradigm-for-human-bot-communication/>

More posts by this contributor

**编者按:***[KITT 的联合创始人兼首席执行官是姚，陈和 Kenji Sagae 是联合创始人。艾](https://web.archive.org/web/20221025224025/http://kitt.ai/)。丹尼尔·李是马德罗纳风险投资集团的合伙人。*

聊天机器人提供了无摩擦获取商品、服务和信息的承诺，但创造有效的机器人可能看起来很棘手。

以无缝、自然的方式与用户互动的机会的另一面是[用户的期望可能高得惊人](https://web.archive.org/web/20221025224025/https://beta.techcrunch.com/2016/05/05/a-few-words-on-chatbots/)。机器人需要智能，并提供比应用程序更大的便利性——这是一种为当今移动设备量身定制的非常有效的 UI 范式，经过十多年的精心完善。

好消息是，认为机器人必须掌握人类语言或取代应用程序才能成功的观点是错误的。机器人将以新的方式与消费者互动，结合人类和机器的优势，允许结构化和非结构化信息自然高效地交换。

## 通信速度

一种简单而直观的衡量沟通有效性的方法是观察单位时间内交换的信息量。在这一框架下，文本(如短信、聊天、电子邮件)和语音(如电话)交互在产生和消耗的信息量上有所不同。

![image001](img/d1b0d4e5228244b165db43e0e19551c9.png)

当我们说话时，通常每分钟产生 120 到 140 个单词，而我们通常每分钟只能写或打 40 到 70 个单词。当我们看信息消耗的速度时，英语阅读速度是每分钟 200 个单词以上，但是听力速度被限制在每分钟 120 到 140 个单词。

短信和聊天应用已经适应了通过自动更正功能和[新型键盘](https://web.archive.org/web/20221025224025/https://beta.techcrunch.com/2016/04/25/microsofts-word-flow-keyboard-app-lands-on-ios/)来提高文本生成速度，但是人类的文本生成总是比消费慢。

然而，想象一下，一个朋友可以以超人的速度输入、绘制、查找信息和查找 gif，并生成按钮、菜单和图片，以加快输入速度。更好的是，您的增强输入对您的朋友来说更容易理解，并且在需要时不会丧失自然语言的灵活性和熟悉度。

我们可能还没有完全做到这一点，但是我们已经非常接近了，尤其是在某些平台上构建良好的机器人。在这里，我们来看看不同机器人平台的特性，这些特性正在将人与机器人的交流塑造成一种更加高效、健壮和自然的用户界面范例。

## 快速回复按钮

快速回复按钮是节省用户时间和防止意外输入的一种简单方便的方式。它们是人-机器人通信的独特之处，因为按钮对于机器人来说很容易创建，对于人类来说也很容易使用；好处包括提高通信速度和机器人理解。

脸书、电报和 Kik 机器人都有快速回复按钮，但名字略有不同，一些机器人，如 Kik 上的丝芙兰机器人，使用快速回复按钮作为主要的交流方式。Slack 仍然缺少快速回复按钮，但是有相关动作的消息按钮。

[电报定制键盘](https://web.archive.org/web/20221025224025/https://core.telegram.org/bots#keyboards):

![image002](img/a4d093043ef58a213c5fb1e2727c1fe9.png)

[Facebook Messenger 快速回复](https://web.archive.org/web/20221025224025/https://developers.facebook.com/docs/messenger-platform/send-api-reference/quick-replies):

![image003](img/9804f22a1c5add4a17690d5db814d883.png)

Kik 建议响应键盘:

![image004](img/4c32e0d5bc3d2ffc3e2f578e28d3c3ef.png)

## 回拨按钮

回拨按钮类似于快速回复按钮，但允许更广泛的潜在交互。当单击回调按钮时，它会生成一个对注册的 webhook 的 HTTP 调用，从而触发预定义的操作。回调按钮是提供反馈的一种很好的方式，它们也为 bot 后端提供了更深入的分析机会。

[松弛信息按钮](https://web.archive.org/web/20221025224025/https://api.slack.com/docs/message-buttons):

![image005](img/d089725ff61ea6c6ac34fd85398e1420.png)

[信使回发按钮](https://web.archive.org/web/20221025224025/https://developers.facebook.com/docs/messenger-platform/send-api-reference/button-template):

![image006](img/c386f97dcf4f522ddde5b22b270b9061.png)

[电报回拨按钮](https://web.archive.org/web/20221025224025/https://core.telegram.org/bots/2-0-intro#callback-buttons):

![image007](img/2da757853bee53224587673cde545046.png)

## 结构化信息共享

共享易于编程解析的信息使得结构化信息的交换从单一语言范式中的笨拙变为混合范式中的简单和明确。

例如，共享一个像“3rd & Madison”这样的位置对于人类和机器来说是模糊且缓慢的，而共享的 GPS 坐标可以通过地图服务快速显示并被机器人理解。

电报[发送联系人](https://web.archive.org/web/20221025224025/https://core.telegram.org/bots/api#sendcontact)和[发送地点](https://web.archive.org/web/20221025224025/https://core.telegram.org/bots/api#sendlocation):

![image008](img/9198363ad4b31f71c47d33ed9faa147b.png)

[Facebook Messenger 位置分享](https://web.archive.org/web/20221025224025/http://newsroom.fb.com/news/2015/06/a-new-way-to-send-a-location-in-messenger/):

![image009](img/7c9e703f10471330fd2831f7444453e7.png)

## 机器人提到

内嵌机器人是一种在聊天过程中快速获取、发送和分享信息的好方法，无需跳出当前界面(去另一个聊天)或当前应用(去另一个应用)。

代替多次点击和菜单来执行一个特定的功能，机器人上的一个@提示音允许一行交互。允许机器人彼此共享会话环境也大大提高了交互速度，因为用户不再需要为每次通信重新输入数据。

[电报内嵌机器人](https://web.archive.org/web/20221025224025/https://telegram.org/blog/inline-bots):

![image010](img/fe9cdaa44841229f428bfd90ed78582e.png)

[Slack Bot 提及](https://web.archive.org/web/20221025224025/https://api.slack.com/bot-users):

![image011](img/29f0f6aa3dd59c232acb4a3d96d0009d.png)

下表总结了四个流行的聊天和机器人平台提供的附加语言触摸功能。这些功能代表了一种混合通信模式的开始，这种模式将使与机器人的通信更加高效和有效:

*   快速回复按钮:节省用户时间，提高机器理解能力
*   回调按钮:提供行动号召和后端分析
*   结构化信息共享:轻松共享机器可读信息
*   提到机器人:让机器人总是存在并且容易被访问

![image012](img/dc3260e496150faf26555d7da6b2ccdb.png)

如果你的机器人没有使用语言触摸混合通信模式，还有其他几种方法可以从按钮和回调中获取一些 UI 机制来构建一个更好的机器人:

*   构建您的系统时，从人开始，找出最常见的沟通模式和该模式的例外情况
*   优化快速和慢速两种渠道沟通的对话，提供清晰、明确的回应(例如，“[回复“是”购买](https://web.archive.org/web/20221025224025/http://replyyes.com/)”)或开放式信息(“你能告诉我泰勒·斯威夫特的新唱片什么时候发行吗？”)
*   使用回调函数，即使没有本机集成。对于更复杂的任务，让用户退出聊天，将他们转移到更适合手头任务的点击或触摸界面
*   考虑迁移到一个更适合新的人机交互的平台

在机器人实现人类级别的通信之前，人工智能和自然语言处理还有[很长的路要走](https://web.archive.org/web/20221025224025/https://beta.techcrunch.com/2016/07/06/key-trends-in-machine-learning-and-ai/)。然而，在此之前，人机交流的新方法将利用人类和机器的优势来创建新的交互范式，就像我们自己的语言一样自然。