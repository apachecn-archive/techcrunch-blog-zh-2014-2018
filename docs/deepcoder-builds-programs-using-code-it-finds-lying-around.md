# DeepCoder 使用它在 TechCrunch 上找到的代码构建程序

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/23/deepcoder-builds-programs-using-code-it-finds-lying-around/>

# DeepCoder 使用它发现的代码构建程序

像所有伟大的程序员一样，我的大部分代码来自 StackOverflow 问题。想不通怎么给 Flask 加认证？[容易](https://web.archive.org/web/20221202124945/http://stackoverflow.com/questions/6972999/flask-user-authentication)。想要关闭 sendmail 吗？[轰](https://web.archive.org/web/20221202124945/http://stackoverflow.com/questions/10359437/sendmail-how-to-configure-sendmail-on-ubuntu)。现在，由于互联网上的所有代码，机器人可以像 18 万美元的编码员一样聪明。

这个名为 [DeepCoder](https://web.archive.org/web/20221202124945/https://openreview.net/pdf?id=ByldLrqlx) 的系统，基本上是搜索一个代码集来构建一个符合规范的项目。它已经被用来完成编程竞赛，并可以针对更大的数据集来构建更复杂的产品。

来自报纸:

￼building IPS 系统需要解决两个问题。首先，搜索问题:为了找到一致的程序，我们需要搜索一组合适的可能程序。我们需要定义集合(即程序空间)和搜索过程。二、排序问题:如果有多个程序符合投入产出实例，我们返回哪一个？这两个问题都依赖于问题表述的细节。因此，制定程序综合方法的第一个重要决定是选择领域特定语言。

随着不断练习，系统变得越来越聪明，找出哪些代码片段在一起工作得最好，以及何时用某个代码片段代替另一个代码片段。因为它“学习”系统可以越来越快，因为它建立更多的程序。

剑桥大学的 Matej Balog 和微软研究院的 Alexander L. Gaunt、Marc Brockschmidt、Sebastian Nowozin、Daniel Tarlow 共同开发了这一产品，并就其使用撰写了一篇论文。程序员注意到，像这样的系统无法用小代码片段构建更大的项目，公平地说，这听起来像是呼啸而过的墓地。

鉴于这是许多程序员的工作方式——切割代码并重新利用它——这似乎是深度学习系统的一个很好的用途。我可以想象这对于简单的 CRUD 应用程序来说是一个很好的解决方案——更新和添加记录到数据库所需的基本工具。事实上，这可能意味着初级程序员工作的终结。就我而言，欢迎我们的人工智能机器人霸主。