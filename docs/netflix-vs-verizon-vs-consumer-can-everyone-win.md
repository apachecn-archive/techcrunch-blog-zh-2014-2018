# 网飞对威瑞森对消费者:谁赢了？

> 原文：<https://web.archive.org/web/http://techcrunch.com/2014/09/06/netflix-vs-verizon-vs-consumer-can-everyone-win/>

**编者按:** *Dror Gill 是 [Beamr](https://web.archive.org/web/20230327095322/http://beamr.com/) 的首席技术官，这是一家为网络出版商、数字分销商、社交网络和媒体公司提供支持的成像技术公司，致力于降低与存储和传输媒体文件相关的成本。*

今天的消费者比以往任何时候都在流式传输更多的视频。仅网飞在过去两年就增加了 2000 多万用户，截至 2014 年 Q2 青奥会用户总数达到 5000 万。难怪视频消费的增长对流媒体服务和互联网服务提供商并不是没有影响。

新闻媒体最近强调了威瑞森和网飞之间旷日持久的争端，网飞指责威瑞森的网络拥堵，未能提供为网飞客户提供高质量服务所需的稳定带宽。网飞甚至向其客户发送信息，指责他们在威瑞森网络上的糟糕体验。

最终，威瑞森[提交了一份停止和终止](https://web.archive.org/web/20230327095322/http://www.foxbusiness.com/technology/2014/06/05/verizon-sends-cease-and-desist-letter-to-netflix-over-slowdown-notices/)文件，迫使网飞撤回了这些信息，威瑞森指责网飞因其有限的交通提供商选择而导致持续的交通问题。威瑞森负责监管事务的副总裁大卫·杨甚至在一篇博客文章中展示了下图，声称威瑞森自己的网络没有拥塞，只是通过他们选择的中转提供商从网飞到威瑞森的链路出现了拥塞。

![Source: Verizon](img/0130e399b7d1dad76b449f0fe2056b2c.png)

资料来源:威瑞森

争论仍在继续，网飞声称威瑞森应该升级其与这些公交提供商的连接，以解决瓶颈问题。Young 立即回答说，网飞应该使用付费对等网络，并为流入其网络的入站流量向威瑞森付费。战斗仍在继续。

这场争论只是互联网瓶颈问题的开始。不仅像 YouTube 和网飞这样的点播视频服务现在占据了整个北美互联网流量的 50%以上，而且思科最近在其[视觉网络指数](https://web.archive.org/web/20230327095322/http://www.cisco.com/c/en/us/solutions/collateral/service-provider/ip-ngn-ip-next-generation-network/white_paper_c11-481360.html)报告中报告说，到 2018 年，视频将占全球消费者互联网流量的 79%。

无论流媒体服务和互联网服务提供商最终是否签署对等协议来解决纠纷，视频带宽问题仍有几种可能的解决方案。一个明显的方法是降低视频比特率，以降低流式视频文件的带宽要求。然而，由于视频质量与分配给视频流的比特率直接相关，盲目降低比特率将导致糟糕的观看体验和不满意的客户——在视网膜显示器和 UHD 4k 电视的时代，这种选择是不可接受的。

另一种解决方案是在网络边缘缓存最常观看的视频文件。这确保了当用户请求流行的视频文件时，它可以从靠近用户的物理位置的位置流出，而不必再次通过互联网主干传输。由于大部分在线视频流量是由相对较少的流行流产生的，当考虑到缓存文件的存储成本与通过网络传输的每个副本的交付成本时，缓存这些流可能是经济高效的。

自适应比特率流是内容传送网络使用的另一种常见解决方案。这种方法实时检测用户的带宽和 CPU 容量，然后相应地调整视频流的质量，以防止用户的连接因比特率超过其处理能力而过载。虽然这种策略会导致额外的存储和编码成本，但它可以消除缓冲，并在高端和低端连接上提供一致的流。

最后，还有媒体优化，它采用已经压缩的视频流，分析其感知属性，并将其编码为较低的比特率，以提高流媒体速度，而不影响原始视频质量。这就像拿一个模型粘土球，挤压它使它变小:它仍然有同样数量的粘土，但是占据了更少的空间。某些形式的媒体优化可能难以在降低文件大小的同时保持视频质量，但当使用可靠的感知质量测量正确完成时，此过程可以将比特率和文件大小降低 20-50 %,同时保留完整的感知质量。

在这些主要参与者继续解决拥塞问题的同时，利用缓存、自适应比特率流和媒体优化等当前解决方案可以缓解带宽瓶颈问题，同时为内容提供商、电信公司和最终用户提供三赢局面。