# 最新的 Chrome Beta 版让开发人员对触摸输入有了更多的控制，增加了新的 JavaScript 特性和不固定的阴影 DOM

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/04/10/google-launches-chrome-beta-35/>

谷歌今日[发布](https://web.archive.org/web/20221006044221/http://blog.chromium.org/2014/04/chrome-35-beta-more-developer-control.html)最新[测试版 Chrome 35](https://web.archive.org/web/20221006044221/https://www.google.com/landing/chrome/beta/) 。虽然在这个版本中没有任何针对最终用户的主要新功能，但该公司为开发人员在其浏览器中添加了广泛的新功能，从长远来看，这些功能将使 web 应用程序在 Chrome 中运行得更好。

一旦开发者实现了它，用户可能首先注意到的特性是支持许多触摸和缩放输入的新属性。例如，在新的[触摸动作 CSS 属性](https://web.archive.org/web/20221006044221/https://groups.google.com/a/chromium.org/forum/#!topic/blink-dev/sc5lHnlcLvM)的帮助下，开发者现在可以在他们的部分内容上禁用触摸滚动、捏放缩放和双击缩放。谷歌表示，这将让开发者对移动设备上经常令人讨厌的 300 毫秒点击延迟有更多的控制，并允许他们创建更可靠的侧扫 ui 和指针事件的聚合填充。

对于桌面用户，该版本引入了一个系统，当控制键被按下时，允许网络应用接收[鼠标滚轮事件](https://web.archive.org/web/20221006044221/https://groups.google.com/a/chromium.org/forum/#!topic/blink-dev/BW4hshtMsmo)。现在，当你使用滚轮并按住 Control 键时，Chrome 会放大和缩小页面。对于包括谷歌地图在内的一些网站来说，这不是正确的行为，所以开发者现在可以基于这个输入调用其他操作。

Google 在这个版本中也取消了对影子 DOM 的访问。影子 DOM 是 Web 组件工作的一个基本特性。根据 Google 的说法，它“T12 为 web 平台带来了用户界面元素的可靠组合”，并允许开发人员和 web 框架“T13 不再担心他们的小部件通过使用冲突的 CSS 选择器、类或 id 无意中破坏页面，并开始依赖 DOM 作为构建组件的可互操作方式。

[https://web.archive.org/web/20221006044221if_/https://www.youtube.com/embed/pQOuHNm5seY?feature=oembed](https://web.archive.org/web/20221006044221if_/https://www.youtube.com/embed/pQOuHNm5seY?feature=oembed)

视频

此次更新的另一个新特性是支持 [ECMAScript 6 标准](https://web.archive.org/web/20221006044221/http://en.wikipedia.org/wiki/ECMAScript)下的大量新 JavaScript 特性。JavaScript 是该标准最著名的实现，ECMASCript 6 将于今年年底发布。不过，谷歌已经开始实现它的一些功能，包括支持像 [JavaScript promises](https://web.archive.org/web/20221006044221/http://www.html5rocks.com/en/tutorials/es6/promises/#toc-async) (一个类似于 JQuery 的[deferres](https://web.archive.org/web/20221006044221/http://api.jquery.com/category/deferred-object/)的功能)、 [WeakMaps](https://web.archive.org/web/20221006044221/https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakMap) 和 [WeakSets](https://web.archive.org/web/20221006044221/https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakSet) 用于创建垃圾收集数据结构和 [object.observe](https://web.archive.org/web/20221006044221/http://updates.html5rocks.com/2012/11/Respond-to-change-with-Object-observe) 用于观察 JavaScript 对象的变化。

然而，这个版本不仅仅是增加新的功能。谷歌也删除了一些功能。它这样做是为了简化其代码库和最小化攻击面，但该公司表示，反对意见主要是关于发展 web API 面“以满足当今用户和开发者的需求。”此版本中不推荐使用的功能包括 Linux 上的传统 web 通知和 NPAPI 支持。你可以在这里找到完整的列表[。](https://web.archive.org/web/20221006044221/http://blog.chromium.org/2014/04/chrome-35-beta-more-developer-control.html)

图片鸣谢:[SW 怀疑论者](https://web.archive.org/web/20221006044221/https://www.flickr.com/photos/swskeptic/7578987062/in/photolist-cxJhNJ-7xumy6-7xybkS-8tomsB-8trnxm-5GRbsV-7qr3Sz-6hdFJ2-5W1V7T-azAMrA-9h25wC-cxJhRQ-5mC748-6SpK9x-7nGPcp-atkFEN-6DdxEh-7oCtYc-7wWr66-7oGmGU-527RA3-7gXRqH-87bQBt-9grHEi-29bzhF-67x6t7-cb3ZZy-aL27Pc-9vzs9s-7tFUGZ-7tKSJY-6hL6UQ-4vsysa-4zmhRz-4H546d-7x1e1o-fA7tMf-7N5e3X-4zmhSX-4zqxkG-4H53Nf-4GZSMD-a3NndE-gsJmkU-5D3zmH-5D3zoP-5D3zwH-5D3zrM-5D7SfG-5D7Sgw)下 [CC BY-SA 2.0 许可](https://web.archive.org/web/20221006044221/https://creativecommons.org/licenses/by-sa/2.0/)。