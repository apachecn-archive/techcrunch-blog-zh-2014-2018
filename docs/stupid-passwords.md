# 阿什利麦迪逊黑客最新提醒愚蠢的密码是愚蠢的 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/09/07/stupid-passwords/>

# 阿什利麦迪逊黑客最新提醒愚蠢的密码是愚蠢的

最近， [fembot 约会](https://web.archive.org/web/20230130230959/https://techcrunch.com/2015/08/31/ashley-madison-refutes-claims-that-its-site-was-populated-with-fake-female-accounts/) 婚外情网站 Ashley Madison 的[黑客攻击](https://web.archive.org/web/20230130230959/https://techcrunch.com/2015/07/20/hackvisitkarma/#.uyoi2s:MT2Z)，导致数百万账户的[数据被转储到网上](https://web.archive.org/web/20230130230959/https://techcrunch.com/2015/08/19/ashley-madison-data-dumped/)，这又给了我们一个有益而熟悉的教训:即使加密得非常好的愚蠢密码也仍然是愚蠢的。

虽然 Ashley Madison 的业务和运营的许多方面都令人惊讶，但该公司显然为其用户密码使用了可靠和受尊敬的加密技术。但是如果用户选择一个愚蠢的密码，比如，呃，password，即使是 bcrypt-hashed 密码也可以被破解。或者 123456。

是的，你可以看到这是怎么回事…

果然，在运行密码破解工具 hashcat 大约两周之后，安全公司 Avast 已经能够破解 25，393 个独特的哈希，其中有 1，064 个独特的密码。

需要明确的是:这是独一无二的密码，因为“不同于迄今为止它能够破解的其他密码”，而不是“多么神奇的密码！“这太复杂了，可能无法破解，”。

该公司一直在使用两个已知的密码列表进行破解:[有史以来最糟糕的 500 个密码](https://web.archive.org/web/20230130230959/http://www.whatsmypass.com/the-top-500-worst-passwords-of-all-time)(始于 2008 年)；以及 2009 年 [RockYou hack](https://web.archive.org/web/20230130230959/https://techcrunch.com/2009/12/14/rockyou-hack-security-myspace-facebook-passwords/) 泄露的 1400 万密码列表。

根据目前能够破解的数据，排名前 20 位的阿什利·麦迪逊密码如下…

1.  123456
2.  密码
3.  12345
4.  12345678
5.  标准英语打字键盘的
6.  猫咪
7.  秘密
8.  龙
9.  欢迎
10.  精力
11.  活泼的
12.  帮助我
13.  口交
14.  尼科尔
15.  贾斯廷
16.  卡马罗
17.  约翰逊
18.  雅马哈商标
19.  午夜
20.  克莉丝

那就不奇怪了。也许除了为什么这么多尼科尔斯？

请记住，上面的密码列表只是来自第一批 100 万个 Ashley Madison 密码的子集，这些密码更有可能是在该网站历史的早期创建的——它大约在 2001 年推出，所以第一批 100 万个密码可能反映了一些非常古老的密码思想。或者不是。

可以说，与第一个一百万相比，最后的一百万个密码可能是一个更有趣的数据测试——看看人类在过去 15 年里是否在创建密码方面有所进步。尽管 Avast 强调这是假设密码数据库是按时间顺序排序的，所以“不能 100%确认”任何一种方式。

有一件事永远是清楚的:人类的第一个冲动是创造一个他们确信会记住的密码，所以愚蠢的密码基本上是人脑存储限制的永恒表现。解决这个问题需要 A)一些其他的技术，B)无论是什么技术，都必须以这样一种方式实现，即使用它比调用和键入 123456 更省力。