# 脸书揭开其移动设备测试实验室 TechCrunch 的面纱

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/07/13/facebook-lifts-the-veil-on-its-mobile-device-lab/>

本周早些时候，脸书带领一小群记者参观了其数据中心。在这个过程中，该公司还展示了其移动设备实验室，用于在物理设备上测试新的 iOS 和 Android 版本的脸书应用程序 Messenger 和 Instagram。

[![device_testing_lab_facebook](img/7e5bf3929ee2265dd7086faec27d3ccf.png)](https://web.archive.org/web/20230131132854/https://techcrunch.com/wp-content/uploads/2016/07/device_testing_lab_facebook.jpg) 移动设备实验室目前占据了数据中心的 60 个机架。每个机架可以容纳 32 部手机，总共将近 2000 个设备，但是，正如脸书的 Antoine Reversat 告诉我们的，计划是将这个数字增加到每个机架 64 个设备。

每个机架都有自己的 Wi-Fi 信号，同时也是一个 [EMI 外壳](https://web.archive.org/web/20230131132854/https://en.wikipedia.org/wiki/Electromagnetic_interference)，以确保相邻机架不会接收到来自其邻居的 Wi-Fi 信号。

每当工程师对脸书的一个主要移动应用程序进行更改时，该应用程序的新版本都会在这些设备上自动测试，以确保不会出现崩溃或性能问题。

可用的设备从基本的 Android Galaxy 手机到最新的 iPhones 都有。正如 Reversat 指出的那样，这些设备也运行各自不同版本的操作系统。对于 Android，这是从 KitKat 开始的所有最新版本，对于 iOS，这是 iOS 7 到 9(我假设该团队也已经在测试 iOS 10)。

为了确保测试的可比性，每次测试后手机都会重启。

所有的电话还需要连接到 PC 或 Mac 上，以便接收最新的代码。正因为如此，每个机架下都有 PC 和 Mac Mini。脸书使用每机架八台 Mac Minis 进行 iOS 测试(因为每台只能与四台 iPhones 通话)，或者使用四台 [OCP Leopard 服务器](https://web.archive.org/web/20230131132854/http://www.opencompute.org/wiki/Server/SpecsAndDesigns)测试 Android 设备。

【T2![DSC06588](img/cc5354640f80d763a7c2328889de6136.png)

但是为什么选择在设备上测试呢？因为有很多模拟器更容易操作。脸书团队认为，虽然模拟器善于找出应用程序可能无法正常工作的原因，但它们不适合性能测试。Reversat 在今天的正式声明中说:“例如，我们无法在模拟器中追踪 1%的性能回归。”“所以我们选择了设备上测试。”

虽然除了使用 [Chef](https://web.archive.org/web/20230131132854/https://www.chef.io/chef/) 之外，脸书并没有说太多关于它如何将更新推送到手机的信息，Reversat 指出，设备实验室源于该公司对 [CT 扫描](https://web.archive.org/web/20230131132854/http://code.facebook.com/pe)的研究，这是该公司去年[首次谈到的一项性能监测服务](https://web.archive.org/web/20230131132854/https://code.facebook.com/posts/924676474230092/mobile-performance-tooling-infrastructure-at-facebook/)。早期，工程师会在单个设备上测试应用程序，但考虑到目前市场上有这么多手机和平板电脑，这根本无法扩展，脸书生产工程组织[的一个小团队开始建造这些机架。](https://web.archive.org/web/20230131132854/http://code.facebook.com/pe)

[gallery ids="1351886，1351879，1351880"]

这些机架的最早版本非常简单，工作效果并不好(很大程度上是因为它们是由金属制成的，过多的金属意味着 Wi-Fi 信号不再有效)。该团队还尝试用 240 个设备建造一堵墙，但这占用了太多空间。

该公司目前在普赖恩维尔使用的最新版本的移动设备架也具有一个摄像头，可以跟踪设备上发生的事情，尽管该团队似乎还没有完全激活这一功能。

该团队现在正致力于支持每个机架多达 64 个设备，并使向设备推送新代码的过程更加高效。然而，也许更重要的是，该团队还计划开源机架的设计和驱动手机的厨师食谱。

当然，脸书并不是唯一一个经营这种实验室的人。例如，如果你想测试自己的应用程序，你可以选择在类似于 [Xamarin](https://web.archive.org/web/20230131132854/https://www.xamarin.com/test-cloud) (现归微软所有) [Amazon](https://web.archive.org/web/20230131132854/https://aws.amazon.com/device-farm/) 和[Google](https://web.archive.org/web/20230131132854/https://www.chef.io/chef/)(Android 应用程序)的服务上运行它们。

[![fb_data_center-3](img/a4921b0a75929ff2e42f0a4a5ad5c28b.png)](https://web.archive.org/web/20230131132854/https://techcrunch.com/wp-content/uploads/2016/07/fb_data_center-3.jpg)