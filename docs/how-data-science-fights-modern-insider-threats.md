# 数据科学如何对抗现代内部威胁

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/08/25/how-data-science-fights-modern-insider-threats/>

本·迪克森是一名软件工程师，也是

[TechTalks](https://web.archive.org/web/20230310181955/https://bdtechtalks.com/)

.

More posts by this contributor

[内部威胁](https://web.archive.org/web/20230310181955/https://bdtechtalks.com/2016/08/08/the-4-insider-threats-to-watch-out-for/)是公司、组织和政府机构面临的最大网络安全威胁。这是你在[安全会议主题演讲](https://web.archive.org/web/20230310181955/https://www.theguardian.com/technology/2016/aug/08/cyber-security-black-hat-defcon-hacking)中经常听到的，也是你在[数据泄露报告](https://web.archive.org/web/20230310181955/https://www.symantec.com/content/dam/symantec/docs/reports/istr-21-2016-en.pdf)、白皮书和调查中读到的——这些内部威胁变得越来越[难以检测和防范](https://web.archive.org/web/20230310181955/http://www.itproportal.com/2015/05/28/why-insider-threats-difficult-detect/)，以及[更加频繁](https://web.archive.org/web/20230310181955/http://www.darkreading.com/endpoint/latest-research-highlights-growing-insider-threat-in-cybersecurity-landscape/d/d-id/1320962)。

这种看似不可阻挡的增长加剧了当前解决方案的问题和缺点，并证明了对新防御技术的需求，以检测和阻止针对我们的数字匕首。

数据科学——应用数学、大数据分析和机器学习来提取知识和检测模式——是一个新兴的先进技术领域，正在[证明其在网络安全领域](https://web.archive.org/web/20230310181955/https://bdtechtalks.com/2016/07/13/how-predictive-analytics-fights-the-cyberthreats-of-the-future/)的有效性，包括打击内部威胁。以下是它如何在传统解决方案失败的地方取得成功。

## 关注用户行为的需要

云服务和移动技术在公司中的广泛采用极大地改变了 IT 基础架构。

随着企业网络和数字资产的物理边界不再像过去那样清晰，应对内部威胁的重点需要转向保护用户账户。网络安全初创公司 [Gurucul](https://web.archive.org/web/20230310181955/http://gurucul.com/) 的营销副总裁汤姆·克莱尔(Tom Clare)表示:“现在，传统的安全边界已经被移动和云计算抹去，身份已经成为攻击媒介和安全边界。

F-Secure Labs 的首席研究员 Jarno Niemel 说:“最近发生的变化是，控制用户账户已经变得比控制设备更有价值。“几年前，我们为了保持计算机清洁而与保持计算机清洁免受感染作斗争。如今，我们保护计算机只是为了能够保护计算机上的用户帐户。”

各种组织通过采用不同的安全解决方案和对员工进行网络安全的[基础培训来努力保护用户身份，但这还不够。](https://web.archive.org/web/20230310181955/https://bdtechtalks.com/2015/12/04/cyber-security-101-simple-measures-everyone-should-adopt/comment-page-1/)

“良好的数据卫生至关重要，但这还不够，” [Interset](https://web.archive.org/web/20230310181955/https://www.interset.com/) 的首席技术官 Stephan Jou 说。“疏忽大意的员工不太可能因为培训而改变，第三方攻击者通常可以在以员工为中心的流程之外进行操作。更重要的是，为间谍活动而窃取信息的内部人员有打破规则的动机。”

> 内部威胁变得越来越难以检测和防范，也越来越频繁。

事实是，凭据盗窃确实会发生，而且经常发生。事实上，一份[威瑞森 2015 年数据泄露报告](https://web.archive.org/web/20230310181955/http://www.computerworld.com/article/2910947/data-security/reading-between-the-lines-verizon-2015-data-breach-investigations-report.html)发现，大多数已确认的安全事件都是由于用户账户受损造成的。大量的用户证书和密码在黑网上低价出售，而且，只要支付很少的费用，任何人都可以访问各种企业网络和云服务，并冒充合法用户。

因此，对抗内部攻击的关键在于检测异常的用户行为。但这再次提出了自己的一系列挑战，因为定义正常和恶意行为不是一门精确的科学，涉及许多错综复杂的问题。

传统的安全防御依赖于对用户活动设置静态规则和警报，以便定义和识别危害指示器(IOC)。但是，当应用于数十、数百和数千用户时，这种模式最终会产生嘈杂的洪水，安全团队不得不浪费时间，并且必须整理大量不重要的事件，这些事件大多是误报。同时，操作不一定解释意图，精明的攻击者将能够通过将恶意活动保持在定义的规则集内来掩盖它们。

使用数据科学有助于从静态模型转向动态模型，动态模型能够根据身份、角色和工作环境定义正常的用户行为。这种方法在减少误报和突出真正导致恶意活动的行为方面非常有效。

网络安全公司越来越多地利用这项技术来应对内部威胁。

## 通过机器学习分析用户行为

Gurucul 的[风险分析](https://web.archive.org/web/20230310181955/http://gurucul.com/gurucul-risk-analytics)安全平台将机器学习模型与大数据相结合，以了解正常的行为基准并发现异常，并提供跨身份、帐户、访问和活动的可见性。“这种行为分析方法，有时被称为用户行为分析或 UBA，可以检测超额访问权限和活动，定义角色并检测未知威胁，”Gurucul 的 Clare 说。

> 云服务和移动技术在公司中的广泛采用极大地改变了 IT 基础架构。

Gurucul 的风险分析还从内部和云环境中收集和监控基于身份的数据和活动。它的机器学习算法，包括自我学习和训练行为轮廓算法，会查看每一笔新交易，并对其进行风险评分。使用聚类和离群值机器学习使可疑行为从其他良性活动中脱颖而出。

Gurucul 的特点之一是它的[动态对等组](https://web.archive.org/web/20230310181955/http://gurucul.com/blog/user-behavior-and-inside-threat-detection)的概念。系统会根据用户通常执行的活动类型以及他们拥有的身份和权限类型自动对用户进行分组。这允许更紧密的行为聚类和更好的突出行为模式中的异常活动的机会。

因此，如果一名销售人员正在下载大量的公司数据，目的是为了以后将其交给竞争对手，即使他们有合法的权限访问这些信息，他们也会脱颖而出，成为调查的目标，因为他们的行为偏离了他们的同行。

## 内部威胁检测背后的数学原理

Interset 是另一个网络安全平台，它依靠半监督机器学习和高级行为分析来检查和关联分散的数据，以发现内部威胁。它的平台分析来自多个来源的数据，这些数据与网络之间或网络内部的数据移动有关，同时还收集有关所涉及的实体的信息，包括用户、端点和应用程序。

Interset 的[数据科学模型](https://web.archive.org/web/20230310181955/http://go.interset.com/l/80502/2016-08-10/3x69bt/80502/76640/Interset_Verizon_DBR___Data_Science.pdf)背后的数学基于三个关键理念。首先，它用概率模型或风险因素取代了传统的布尔警报。发出概率的模型比真/假警报更有效，并允许使用数学将不同数据集的多条证据结合起来，以确定用户帐户被泄露或参与非法活动的可能性。

其次，它使用机器学习根据收集的数据为每个参与者定义动态阈值，这是一个比全球应用的规则(如“允许多少兆字节的附件”)更灵活的模型。通过分析用户生成的数据产生的“数学指纹”使得识别异常行为变得更加容易。

> 转向数据科学等新技术有助于大海捞针。

第三，该平台脱离了事件层面，使用数学来关联、确证和汇总事件，以将风险归因于更高级别的参与者。这种模式的结果是能够命名名称，即确定谁在窃取数据，而不是找出数百个交易事件中的哪一个表明数据正在被窃取。

根据 Interset Jou 的说法，这个平台“可以在几个小时内发现并揭露爱德华·斯诺登的活动。”

## 用人类专业知识补充分析

F-Secure 的 Niemel 解释说:“从技术的角度来看，我们正在研究用户帐户进行的操作，无论是由帐户的原始所有者进行的恶意操作，还是有人能够危害所述帐户，都没有多大关系。”

这家芬兰公司的最新安全产品，[快速检测服务](https://web.archive.org/web/20230310181955/https://www.f-secure.com/en/web/business_global/rapid-detection-service) (RDS)，是一个抵御内外威胁的平台。Niemel 称之为“一个能够检测内部人员和攻击者的系统，这些人能够破坏一些用户帐户，实际上是一个‘内部人员’。”

托管服务结合使用威胁情报、大数据分析、机器学习和安全专家来提供关于安全警报的准确、可操作的数据，并检测内部威胁的异常和迹象。

“从统计学的角度来看，大多数用户在他们的工作中有相当清晰和重复的模式，”Niemel 说。因此，在试探法和机器学习系统的支持下，可以用适当的接近实时的统计分析工具来检测用户行为的惊人变化。"

> 组织通过采用不同的安全解决方案和对员工进行网络安全基础知识的培训来努力保护用户身份，但这还不够。

RDS 从不同来源收集数据，包括来自公司端点的行为信息，并检测用户帐户何时开始以异常方式运行。近实时分析、存储数据分析和大数据分析的使用使 RDS 平台能够将用户行为与基准标准、历史数据和已知威胁进行比较，以便检测恶意活动的迹象，同时过滤掉误报。

F-Secure 方法的独特之处在于，它的人类专家团队会对其机器学习引擎检测到的异常情况进行验证并提供事件响应。确认违规后，会联系并通知客户。

## 放大恶意内部活动以方便检测

安全供应商的安全运营主管 Greg Foss 解释说: [LogRhythm](https://web.archive.org/web/20230310181955/https://www.crunchbase.com/organization/logrhythm#/entity) 从稍微不同的角度处理内部威胁，并认为对手可能已经突破了边界，因此我们的检测主要侧重于在攻击者进入后跟踪他们的活动

*该公司的[用户威胁检测](https://web.archive.org/web/20230310181955/https://logrhythm.com/solutions/security/user-behavior-analytics/)模块通过蜜罐分析和开源蜜罐解决方案提供内部威胁检测能力。[蜜罐](https://web.archive.org/web/20230310181955/https://www.sans.org/security-resources/idfaq/what-is-a-honeypot/1/9)是引诱恶意黑客的诱饵或网络陷阱，使安全软件能够检测、转移或抵制他们的邪恶活动。*

 *LogRhythm 研究了[蜜罐、欺骗和敏感文件跟踪](https://web.archive.org/web/20230310181955/http://www.crn.com/news/security/300077992/the-art-of-deception-new-class-of-security-startups-use-decoys-to-disrupt-a-hackers-movement.htm),以确定欺骗攻击者的方法，并跟踪他们在组织中的活动。Foss 解释说:“诀窍不是让妥协变得不可能，而是确保它是响亮的和引人注目的，以便 SOC 可以检测到威胁并做出响应。”

Foss 还强调网络流量分析是检测内部威胁的另一个关键部分。“很多人问他们应该使用什么威胁源来帮助找到他们网络上的坏人，”Foss 说。“我经常告诉他们，他们已经有了他们需要的一切，他们只需要开始仔细查看他们已经在收集的数据。”

LogRhythm 使用深度数据包分析来调查大量的网络流量，并在恶意内部人员想要泄露敏感信息时抓住他们，同时检测受损的网络节点，如进行数据包捕获活动的[机器](https://web.archive.org/web/20230310181955/https://logrhythm.com/blog/who-is-listening-in-on-your-network/)。

## 应对未来的威胁

随着组织使用越来越多的在线服务并产生比以往更多的数据，内部威胁将变得越来越复杂，越来越难以发现。从传统方法转向数据科学等新方法和新技术有助于大海捞针，加快检测和阻止内部威胁的过程，以免造成不可逆转的损害。*