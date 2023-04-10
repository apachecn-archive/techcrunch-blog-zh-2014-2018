# 黑客接管了 Gentoo Linux GitHub 仓库 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/06/29/hackers-too-over-the-gentoo-linux-github-repository/>

# 黑客接管了 Gentoo Linux GitHub 存储库

据 Sophos 的研究人员称，流行的 Linux 发行版 Gentoo 已经被“完全破解”,当前的代码没有一个是可信的。团队[立即发布了一个更新](https://web.archive.org/web/20230130100805/https://www.gentoo.org/news/2018/06/28/Github-gentoo-org-hacked.html)，并指出没有任何真正的代码被破坏。然而，他们已经撤回了 GitHub 库，直到他们可以上传一份新的未掺杂代码。

“今天，6 月 28 日，大约在世界协调时 20:20，不明身份者控制了 GitHub Gentoo 组织，并修改了那里的存储库内容和页面。我们仍在努力确定确切的范围，并重新获得对该组织及其资料库的控制。所有托管在 github 上的 Gentoo 代码目前都应该被认为受到了威胁，”Gentoo 管理员写道。“这不会影响托管在 Gentoo 基础设施上的任何代码。因为主 Gentoo ebuild 存储库托管在我们自己的基础设施上，而且 Github 只是它的一个镜像，所以只要你使用来自 gentoo.org 的 rsync 或 webrsync 就没问题。”

没有任何代码会被永久损坏，因为 Gentoo 管理员保留了他们自己的代码副本。Gentoo 表示，被入侵的代码可能包含恶意软件和错误，用户应该避免 GitHub 版本，直到它恢复。

“Gentoo 基础设施团队已经确定了入口点，并锁定了受损的帐户，”管理员写道。三个包含 Gentoo 代码的 Github 库， [Musl](https://web.archive.org/web/20230130100805/https://gitweb.gentoo.org/proj/musl.git/) 和 [systemd](https://web.archive.org/web/20230130100805/https://github.com/systemd/systemd) 。所有这些存储库都被“重置回已知的良好状态”。"