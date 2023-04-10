# 安全研究人员发现没有密码的美国陆军机密数据

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/11/28/army-nsa-inscom-aws-leak/>

# 安全研究员发现没有密码的美国陆军机密数据

在最新一期的《啊哈，我们把它放在外面了》中，在一个没有密码保护的云存储服务器上发现了一批美国国家安全局和军队的文件，任何人都可以通过这个网址访问。安全公司 UpGuard [的 Chris Vickery 在一个未上市的亚马逊网络服务 S3 云存储服务器上发现了这些文件](https://web.archive.org/web/20230319175856/https://www.upguard.com/breaches/cloud-leak-inscom)，该服务器属于美国陆军情报和安全司令部(INSCOM)，这是一个情报收集和安全司令部，由美国陆军和国家安全局联合运作。

在这一桶数据中，维克里发现了 47 个可浏览的文件和三个可下载的文件，其中一些文件包含被指定为“绝密”或“NOFORN”的信息，这是一个安全术语，规定材料不应与外国盟友共享。正如 UpGuard 的报告所详述的那样，维克里还发现了“一个用于在安全的联邦 IT 环境中进行通信的虚拟硬盘驱动器”和“关于国防部战场情报平台的细节”，即所谓的 DCGS-A 和红盘上的信息，“一个陷入困境的国防部云情报平台”，集成到红盘中。这次入侵还包括属于 Invertix 的私钥，invert IX 是一家与 INSCOM 合作的国防承包商。有问题的文件存储在一个名为“INSCOM”的子域中。

“虽然 UpGuard 网络风险团队已经发现并帮助保护了多个涉及敏感国防情报数据的数据暴露，但这是第一次明确保密的信息出现在暴露的数据中，”UpGuard 指出。

最近，这种错误配置的存储服务器正在成为安全世界中常见的警示故事。今年早些时候，[的同一名研究人员发现](https://web.archive.org/web/20230319175856/https://arstechnica.com/information-technology/2017/05/defense-contractor-stored-intelligence-data-in-amazon-cloud-unprotected/)一组属于国防承包商博思艾伦公司的敏感文件被遗漏在一台类似的不安全服务器上。当然，问题不在于安全公司正在挖掘这些未受保护的机密材料，而在于我们无法知道还有谁在挖。