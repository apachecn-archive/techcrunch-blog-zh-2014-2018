# 谷歌的人工智能二重奏实验让你和机器一起演奏

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/16/googles-a-i-duet-experiment-lets-you-jam-with-the-machine/>

# 谷歌的人工智能二重奏实验可以让你和机器一起演奏

Google today [推出](https://web.archive.org/web/20230403140600/https://blog.google/topics/machine-learning/play-duet-computer-through-machine-learning/)一个有趣的新机器学习实验: [A.I. Duet](https://web.archive.org/web/20230403140600/http://aiexperiments.withgoogle.com/ai-duet/view) 。这种新的基于网络的实验让你在电脑键盘(或插入电脑的支持 MIDI 键盘)上演奏旋律，然后电脑会尝试与你演奏二重奏。

工作原理是这样的:你基本上弹奏几个音符，然后等待程序返回响应。不过，计算机返回的数据听起来通常非常随机。例如，很明显，你弹奏的音符和你弹奏的速度有一定的关系，但是这种关系并不能准确地转化为旋律或任何接近你弹奏的时间和节奏的东西。但也许这就是电脑喜欢音乐的方式？

尽管如此，偶尔算法会得到正确的结果，你会与机器进行良好的互动，这实际上类似于音乐。

谷歌表示，该实验基于 Tensorflow 的 [Magenta 开源项目](https://web.archive.org/web/20230403140600/https://github.com/tensorflow/magenta)，该项目专注于将机器学习引入音乐和 [Tone.js](https://web.archive.org/web/20230403140600/https://github.com/Tonejs/Tone.js) 。该系统不使用任何预编程算法。相反，它已经在现有的旋律上接受了训练，然后利用这些旋律做出反应。