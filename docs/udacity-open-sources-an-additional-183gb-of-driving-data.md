# Udacity 开源了额外的 183GB 驾驶数据 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/10/05/udacity-open-sources-an-additional-183gb-of-driving-data/>

# Udacity 开源了额外的 183GB 驾驶数据

上个月， [Udacity](https://web.archive.org/web/20230212130022/https://www.udacity.com/) 创始人巴斯蒂安·特龙在 TechCrunch Disrupt 的舞台上宣布，这家在线教育公司将在[制造自己的无人驾驶汽车](https://web.archive.org/web/20230212130022/http://udacity.com/self-driving-car)，作为其无人驾驶汽车纳米学位项目的一部分。为了实现这一目标，Udacity 创造了一系列挑战，以利用社区的力量来制造最安全的汽车——这意味着欢迎任何人和每个人成为开源项目的一部分。[挑战一](https://web.archive.org/web/20230212130022/https://medium.com/udacity/were-building-an-open-source-self-driving-car-ac3e973cd163#.wgnusfuvc)是为相机支架建立一个 3D 模型，但[挑战二](https://web.archive.org/web/20230212130022/https://medium.com/udacity/challenge-2-using-deep-learning-to-predict-steering-angles-f42004a36ff3#.ur6du1kxz)已经将深度学习融入其中。

在最新的挑战中，参与者的任务是使用驾驶数据来预测转向角度。最初，Udacity 发布了 40GB 的数据，以帮助家庭修理工在无法获得谷歌特斯拉(Tesla of Google)拥有的驾驶数据的情况下，构建有竞争力的模型。然而，由于深度学习模型按池塘而不是按加仑喝数据，[该公司额外推出了 183GB 的驾驶数据。](https://web.archive.org/web/20230212130022/https://medium.com/udacity/open-sourcing-223gb-of-mountain-view-driving-data-f6b5593fbfa5#.dhjt52b0z)

完整的 223GB 包包含山景城两天内超过 70 分钟的驾驶数据以及晴天和阴天镜头。各种各样的镜头将提高提交的质量，并为参与者提供更真实的数据，更好地代表现实世界驾驶和不断变化的道路条件的挑战。

这些视频还被裁剪成匹配的数据，如纬度、经度、档位、刹车、油门、转向角度和速度。所有这些信息都将推动卷积神经网络的创建，最终使配有深度学习的相机能够安全地将你从 a 点带到 b 点。

该公司在其 Challenge #2 博客帖子中表示:“通过让汽车自己理解如何解释图像，我们可以跳过手动选择要检测的特征的复杂性，并通过避免基于激光雷达的解决方案，大幅降低自动驾驶汽车上路所需的成本。”。

虽然 223GB 听起来像是一个很大的数据量，但与优步和特斯拉等公司通过自动驾驶汽车积累的大量数据相比，这仍然相形见绌。一些报告显示，复杂的捕获系统每秒钟可以生成近 1gb 的数据，上述公司拥有数百万英里的数据。从本质上来说，这些 Udacity 数据集在大小上要紧凑得多，因为它们只包含基本的数据和视频镜头，但其背景强调了数据在推动下一代汽车的创造方面有多么重要。

当然，这个挑战不仅仅是制造一辆汽车，而是在这个过程中学习。如果这个挑战听起来很有趣，[前往 GitHub](https://web.archive.org/web/20230212130022/https://github.com/udacity/self-driving-car) ，在那里你可以访问 Udacity 的数据集。