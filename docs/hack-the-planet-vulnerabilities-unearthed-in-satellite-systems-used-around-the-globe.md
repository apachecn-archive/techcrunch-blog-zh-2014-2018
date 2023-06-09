# 黑客入侵地球:全球使用的卫星系统中发现的漏洞

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/08/08/hack-the-planet-vulnerabilities-unearthed-in-satellite-systems-used-around-the-globe/>

# 入侵地球:全球使用的卫星系统中发现的漏洞

所以这很糟糕。企业安全公约之王黑帽今天拉开帷幕，在安全研究的连珠炮中最引人注目的是 IOActive 的 [Ruben Santamarta](https://web.archive.org/web/20230318211413/https://www.blackhat.com/us-18/briefings/schedule/speakers.html#ruben-santamarta-31808) 的一些令人印象深刻的工作，他的团队发现了卫星通信系统(又名 SATCOM)中令人担忧的漏洞，该系统被全球的飞机、船只和军事单位使用。

现在，这还不是*灾难性的*坏:特别是，虽然攻击者可以干扰或禁用你的飞行无线网络，可以想象他们试图侵入连接到他们的设备和/或禁用所有飞行卫星通信，但他们实际上无法影响任何控制飞机的系统。更大的担忧是在军事或海洋领域，因为这些是*远程*漏洞——互联网上的任何人都可以侵入一个连接的易受攻击的卫星通信设备。也就是说，大概是大多数人，因为交流是他们存在的全部原因。

在前一种情况下，除了攻击者修改或禁用卫星通信的风险之外，带有机载 GPS 的设备还可能泄露军事单位的位置。在这两种情况下，这打开了“网络物理攻击”的前景，这是一个绝妙的反主题短语，如果曾经有过的话；基本上，如果你通过卫星天线获得足够的能量，它可以辐射足够强大的能量，影响生物组织和电气系统。和微波炉的原理一样。

但是等等，更糟的是！这些是嵌入式系统。一般来说，没有简单的方法向他们传送远程升级；在某些情况下，唯一的升级是大规模更换。虽然有针对航空和军事卫星通信的缓解措施(不是*修复*本身，而是降低攻击严重性和可能性的方法),但海事系统……问题更多。

所以。不要太担心*如果你不是一名水手或士兵，你的飞机不会因此而下降或转向……但是坐在远离地面的电脑前的人可能会接管你的飞行无线网络。Santamarta(他有这种事情的历史)和 IOActive 正在与供应商和未指明的“政府机构”合作解决这些漏洞，但听起来，至少在公海上，这个问题将伴随我们一段时间。*

(关于这些漏洞的完整技术讲座将在明天举行；今天的记者招待会仅仅是一个试探。我会用任何出现的重要细节更新这篇文章。)