# Chromecast 如何在不使用 WiFi 的情况下连接到朋友的手机？超声波 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/06/26/how-can-chromecast-connect-to-your-friends-phones-without-using-wifi-ultrasonic-sounds/>

# Chromecast 如何在不使用 WiFi 的情况下连接到朋友的手机？超声波

在昨天的 I/O 主题演讲中，谷歌宣布 Chromecast 将推出一个相当神奇的新功能:很快，你的朋友将无需连接到你的 WiFi 就可以向你的电视发送东西。只要他们在同一个房间，它应该就能工作。

但是怎么做呢？

虽然谷歌的 Rishi Chandra 昨天提到新的无线配对系统使用了“多种技术”来确定你何时靠近 Chromecast 设备，但他并没有详细说明这些技术可能是什么。蓝牙？谷歌捏造的一些专有协议？*魔法*？

事实证明，它最接近最后一个——或者至少，对任何没有超人听力的人来说，它可能看起来*像是*魔法。

多亏了主题演讲后的介绍，我们现在对它的工作原理有了更好的了解:超声波，人耳听不到。

一旦您将 Chromecast 配置为允许附近的设备连接，Chromecast 将通过电视的扬声器推送独特生成的超声波。声波中的编码是手机配对时需要知道的一切。你听不到这些声音，但你的手机可以。

使用 Chromecast SDK 的应用程序将使用智能手机的麦克风来监听这些声波。一旦检测到一个，它会提供一个 Chromecast 配对按钮，就像你在同一个 WiFi 网络上一样。

听起来熟悉吗？至少在去年，谷歌的工程师们实际上一直在考虑超声波网络[的想法。与此同时，在去年 9 月的 TechCrunch Disrupt SF 上，一家名为 SlickLogin](https://web.archive.org/web/20221209224113/http://smus.com/ultrasonic-networking/) [的公司推出了一种使用超声波](https://web.archive.org/web/20221209224113/https://beta.techcrunch.com/2013/09/09/slicklogin-wants-to-kill-the-password-by-singing-a-silent-song-to-your-smartphone/)进行双因素认证的方法，而无需额外的打字。仅仅五个月后，他们就被收购了。买家呢。[你猜对了:谷歌。](https://web.archive.org/web/20221209224113/https://beta.techcrunch.com/2014/02/16/google-acquires-slicklogin-the-sound-based-password-alternative/)

[通过 [GigaOm](https://web.archive.org/web/20221209224113/http://gigaom.com/2014/06/26/chromecast-will-use-ultrasonic-sounds-to-pair-your-tv-with-your-friends-phones/)