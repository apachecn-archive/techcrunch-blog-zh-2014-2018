# DigitalOcean 添加浮动 IPs，一劳永逸地解决服务器停机问题

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/10/20/digitalocean-adds-floating-ips-to-kill-server-downtime-once-and-for-all/>

# DigitalOcean 添加浮动 IPs，一劳永逸地解决服务器停机问题

流行的云托管服务 [DigitalOcean](https://web.archive.org/web/20230405201937/https://www.digitalocean.com/) 今天刚刚增加了一个非常有趣的功能——[浮动 IPs](https://web.archive.org/web/20230405201937/https://www.digitalocean.com/company/blog/floating-ips-start-architecting-your-applications-for-high-availability/) 。所以你可能会问那是什么，为什么我需要它？它比切片面包好吃，让我告诉你为什么。

许多开发者正在使用这些时髦的云托管服务，如 DigitalOcean、亚马逊网络服务、谷歌云计算和微软 Azure。与优秀的旧服务器相比，它增加了抽象和灵活性。

特别是，如果您想在多个数据中心运行您的应用程序，可以在任何地方复制您的应用程序。但是当你需要管理一个网络时，事情就变得复杂了。替换一个 droplet(云服务器)并不像它应该的那样简单，因为你需要告诉你的其他 droplet，你的一个 droplet 没有相同的 IP 地址。

把它看作是对你的邮件人的主要依赖——他们知道你所在城镇的每个人和所有地址，如果有人搬到了新房子，他们可以帮助你，但也许你不想每次寻找地址时都依赖他们。

遇见浮动 IP。如果我对这些事情理解正确的话，DigitalOcean 的新功能可以让你保留你的 IP，并将其分配给同一数据中心的任何液滴。您的 IP 地址附加到您的帐户，而不是您的实例。我认为这就像亚马逊的 [EC2 弹性 IP](https://web.archive.org/web/20230405201937/https://aws.amazon.com/articles/1346) 功能。

有许多使用案例，但我最喜欢的一个是紧急情况，因为谁不喜欢一部好的灾难电影。假设你的一滴完全分解了。这是不可修复的，否则将需要几个小时来修复。你可以用保存的图像启动一个新的 droplet，并把旧的 IP 分配给新的 IP，而不是调整你的 droplet——我称之为奇迹。

更好的是，您可以运行备份 droplet 来复制您的生产 droplet 所做的一切，而不是从映像中恢复。每当你的生产液滴发生问题，你只需移动 IP 和 *voilà* ！我敢肯定，你甚至可以找到方法脚本一切，所以你不必重新分配手动 IP。

例如，您可以将浮动 IP 用于两个负载平衡器。是不是很棒？DigitalOcean 现在已经为 70 万开发者部署了 800 万台云服务器。不错，一点也不错！