# 数字海洋推出其对象存储服务 Spaces

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/09/20/digital-ocean-launches-spaces-its-object-storage-service/>

# 数字海洋推出了其对象存储服务 Spaces

数字海洋今天宣布了其对象存储服务 [Spaces](https://web.archive.org/web/20230405201823/https://www.digitalocean.com/products/object-storage/) 。这是对该公司块存储服务的补充。当然，这两种服务有不同的用例；[与](https://web.archive.org/web/20230405201823/https://www.digitalocean.com/community/tutorials/object-storage-vs-block-storage-services)块存储服务不同，作为对象存储的 Spaces 可以扩展到远远超过块存储服务的 16TB 限制，因为它不是基于卷的，也不是将存储连接到虚拟机。

对于 Digital Ocean 来说，这标志着其核心云计算服务之外的又一次扩张，并显示了该公司在这个市场上更直接地挑战亚马逊、谷歌和微软等大型竞争对手的雄心(尽管这些公司显然仍然提供比 Digital Ocean 更广泛的服务)。

“对象存储是我们被要求开发的最受欢迎的产品之一，”该公司云存储服务产品经理约翰·甘农在今天的公告中写道。“当我们着手开发一款从计算资源中抽象出来的可扩展存储产品时，我们意识到我们有机会重构和改进开发人员目前解决这一问题的方式。”

该公司还指出，这项服务与现有的许多 AWS S3 工具兼容，所有数据都位于 256 位 AES-XTS 全磁盘加密的磁盘上。当然，开发者也可以在上传之前用他们自己的密钥加密他们的文件。

这项服务的定价非常简单:你每月支付 5 美元，包括 250GB 的存储空间和 1TB 的出站带宽。除此之外，您还需要为每 GB 存储空间支付 0.02 美元，为每 GB 传输空间支付 0.01 美元。Digital Ocean 还为想体验这项服务的开发者提供了两个月的免费试用。

Spaces 现已在该公司的 NYC3 地区推出，并将在年底前抵达 AMS3 地区，更多地区将在 2018 年初推出。