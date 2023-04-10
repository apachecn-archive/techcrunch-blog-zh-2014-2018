# 谷歌开源 Seurat，一个降低移动虚拟现实复杂性的工具 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/05/04/google-open-sources-seurat-a-tool-for-reducing-mobile-vr-complexity/>

# Google 开源 Seurat，一个降低移动 VR 复杂性的工具

今天是谷歌兑现其 2017 年 I/O VR 承诺的日子。该公司刚刚宣布将开源 Seurat，这是一款旨在降低高保真移动 VR 场景复杂性的工具，可大幅提高性能。

此次发布与 [Mirage Solo](https://web.archive.org/web/20221025222428/https://techcrunch.com/2018/05/04/review-lenovo-mirage-solo-headset-with-google-worldsense-tracking/) 的发布同时进行，这是 Daydream VR 平台上第一款使用谷歌 WorldSense 位置跟踪系统的耳机。该耳机是独立的，运行在移动芯片组上，因此比连接到游戏电脑的耳机更受资源限制。

修拉是一个软件工具，旨在减少多边形数量。基本上，修拉考虑了虚拟现实用户可能给予他们有限运动范围的所有可能的视点，并删除了他们永远无法看到的 3D 环境区域。修拉从等式中删除了对象持久性，所以如果你在虚拟现实中看不到它，它很可能实际上根本不存在。

[https://web.archive.org/web/20221025222428if_/https://www.youtube.com/embed/NThgBol6YWs?start=3&feature=oembed](https://web.archive.org/web/20221025222428if_/https://www.youtube.com/embed/NThgBol6YWs?start=3&feature=oembed)

视频

在上面新的《银翼杀手》标题的片段中，谷歌表示，修拉程序能够拍摄 4660 万个三角形的场景，并将其减少到 307000 个。这对于开发人员来说特别有用，他们可以将现有的渲染从功能更强的硬件移植到更紧张的移动 VR 硬件。

该工具的源代码和文档可在其 [GitHub 页面](https://web.archive.org/web/20221025222428/https://github.com/googlevr/seurat)上获得。