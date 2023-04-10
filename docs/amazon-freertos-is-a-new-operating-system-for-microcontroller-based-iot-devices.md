# Amazon FreeRTOS 是基于微控制器的物联网设备的新操作系统 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/11/29/amazon-freertos-is-a-new-operating-system-for-microcontroller-based-iot-devices/>

# 亚马逊 FreeRTOS 是一款面向基于微控制器的物联网设备的新操作系统

当您想到物联网设备时，您可能会想到连接的摄像头或传感器。这些设备中的大多数都有非常基本的 CPU，运行 Linux 或类似的操作系统。然而，并不是每个物联网设备都有真正的 CPU。相反，它们由基本的微控制器驱动。那些设备(想想烟雾探测器，等等。)往往都比较旧，不能直接连上云。他们倾向于运行某种版本的免费操作系统和内核。

正如 AWS 首席执行官 Andy Jassy [今天在公司的 re:Invent 大会上宣布的](https://web.archive.org/web/20230130100805/https://aws.amazon.com/blogs/aws/announcing-amazon-freertos/)，该公司思考了这个问题，并决定以亚马逊 FreeRTOS 的形式建立自己的操作系统。AWS 表示，这是一个微控制器操作系统，旨在简化这些非常基本的物联网设备的开发和安全性。它应该运行在一个低功耗的连接设备上，可以直接或通过 [AWS Greengrass](https://web.archive.org/web/20230130100805/https://aws.amazon.com/greengrass/) 连接到云。

顾名思义，Amazon FreeRTOS 本质上是 FreeRTOS 操作系统的扩展，增加了用于本地和云连接的库。随着时间的推移，亚马逊还将增加对空中更新的支持。