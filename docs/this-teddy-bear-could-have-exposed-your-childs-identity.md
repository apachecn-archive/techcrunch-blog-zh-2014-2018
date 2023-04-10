# 这只泰迪熊可能会暴露您孩子的身份 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/02/02/this-teddy-bear-could-have-exposed-your-childs-identity/>

智能玩具值得冒险吗？这是父母们这些天在权衡云连接玩具的实用性和乐趣时问自己的问题，它们有可能被变成间谍设备，因为[是针对 Wi-Fi 功能的“你好芭比](https://web.archive.org/web/20221226111553/http://www.newsweek.com/privacy-advocates-want-take-wifi-connected-hello-barbie-offline-313432)”的索赔，或者是涉及孩子个人信息的大规模泄露的可能性，就像伟易达数据泄露的情况一样。

今天，这个问题再次成为人们关注的焦点，[安全研究人员披露了费雪公司“智能玩具”中的一个漏洞](https://web.archive.org/web/20221226111553/https://community.rapid7.com/community/infosec/blog/2016/02/02/security-vulnerabilities-within-fisher-price-smart-toy-hereo-gps-platform)，该漏洞可能会将儿童的个人资料暴露给黑客，包括姓名、生日、性别、语言等，并允许劫持儿童帐户来更改他们的用户资料或其他数据。

![heroes-3-3](img/38083cd2779709ea78d3fe70acc751dd.png)

Fisher-Price 的“智能玩具”是一系列数字填充动物，如泰迪熊，它们与互联网相连，以提供个性化的学习活动。针对 3 至 8 岁的儿童，这些玩具实际上适合儿童找出他们最喜欢的活动。他们还使用图像和声音识别的组合来识别孩子的声音，并读取“智能卡”，从而开始各种游戏和冒险。

[根据 Rapid7](https://web.archive.org/web/20221226111553/https://community.rapid7.com/community/infosec/blog/2016/02/02/security-vulnerabilities-within-fisher-price-smart-toy-hereo-gps-platform) 的安全研究人员今天发布的一份报告，这些智能玩具可能已经被黑客破坏，他们想利用底层软件的弱点。具体来说，问题是平台的 web 服务(API)调用没有适当地验证消息的发送者，这意味着攻击者可能发送了不应该被授权的请求。

受影响的 API 包括那些可能列出客户玩具详细信息(玩具 ID、名称、类型、儿童档案)的 APIs 那些允许他们检索孩子的个人资料数据，如他们的名字、生日、性别、语言和他们玩的玩具；还有更多。

黑客也可能做了一些事情，比如修改客户的账户；创建、编辑或删除孩子的个人资料。查看父母是否在使用玩具附带的移动应用程序；并读取其他杂项数据，如客户购买了什么、游戏分数和其他项目。

![Fisher_Price_Smart_Toy_Monkey_Fisher_Price_DNV32_22_res](img/8312e081c9b5ebd9216569d30bdb5ec9.png)

其中一些问题可能令人烦恼，但更令人不安的是，黑客可能已经获取了一个孩子的个人信息——比如他们的名字和出生日期。Rapid7 的马克·斯坦尼斯拉夫在一篇详述安全问题的帖子中说，这是“大多数父母都会担心的事情”。

他解释说:“虽然在特殊情况下，姓名和生日名义上是非秘密数据，但这些数据可以在以后与孩子更完整的个人资料结合起来，以促进任何数量的社会工程或其他针对孩子或孩子的照顾者的恶意活动。”

该漏洞是通过适当的程序披露的，Fisher-Price 在 Rapid7 首次联系后的两个月内解决了该漏洞，该公司报告称，没有迹象表明任何未经授权的个人使用这种方法访问了客户信息。

**玩具黑客和可接受的风险**

值得注意的是，单独黑掉玩具不足以让孩子处于危险之中。

当然，这就引出了一个问题:在购买智能玩具时，父母在可接受的风险方面的底线在哪里？

即使父母完全远离联网玩具，以保护他们的孩子免受*任何*可能的潜在风险，他们可能仍然会在家里堆满其他联网设备，使他们的家庭变得脆弱。如今，人们会购买联网恒温器、烟雾报警器、婴儿监视器、安全摄像头、亚马逊 Echo 之类的扬声器以及其他“智能家居”设备。任何上网的设备都有可能被攻击。

但在泰迪熊黑客事件中，古老的育儿技巧——如教授“陌生人的危险”或使用安全词汇——可以减轻攻击者所带来的风险，攻击者知道了孩子的身份，然后试图以某种有害的方式利用这一点，如绑架。

**这并不意味着这些服务没有被正确锁定是可以接受的**，但是对它们带来的现实世界的危险保持冷静是值得的。

![HereO-family-watch2](img/b1b721c96dd194281ce22977bf1fd045.png)

一些被黑客攻击的设备比其他设备更危险。例如，比泄露数据的填充动物玩具更令人担忧的是 Rapid7 今天的其他披露:家庭定位器/智能手表 hereO 的 GPS 平台中的一个漏洞可能允许攻击者访问每个家庭成员的位置、位置历史，并“随意滥用其他平台功能。”

供应商也对此进行了修补，但显然，获得这些数据的攻击者可能是更大的直接威胁。

也就是说，大多数罪犯选择阻力最小的道路，许多人寻找机会犯罪。

我们[已经](https://web.archive.org/web/20221226111553/http://www.telegraph.co.uk/technology/news/8789538/Most-burglars-using-Facebook-and-Twitter-to-target-victims-survey-suggests.html) [警告](https://web.archive.org/web/20221226111553/https://techcrunch.com/2010/02/17/please-rob-me-makes-foursquare-super-useful-for-burglars/) [有](https://web.archive.org/web/20221226111553/http://abc7news.com/travel/burglars-use-social-media-to-find-next-victims/448107/)年了，度假时发布社交媒体更新会引来窃贼。然而，实际的例子中，[已经很少](https://web.archive.org/web/20221226111553/http://www.cnet.com/news/twitter-user-says-vacation-tweets-led-to-burglary/)和[在](https://web.archive.org/web/20221226111553/http://www.wmur.com/Police-Thieves-Robbed-Homes-Based-On-Facebook-Social-Media-Sites/11861116)之间了。毕竟，监视一所房子比搜索推特或脸书更容易。同样，大多数想要绑架儿童的罪犯也不太可能花几个小时来破解你的小玩意或玩具。担心玩具黑客可能会偏离现实，即陌生人绑架很少发生。在四分之三的情况下，家庭成员或熟人应该受到责备。

有时候，真正的危险不是潜伏在互联网另一端的陌生人，而是你已经允许进入你的家庭和生活的人。