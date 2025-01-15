# 安装 r2modman
---

!> 请注意：如果您在使用r2modman之前曾使用过其他长号冠军相关mod，请在安装完r2modman之后查阅 [数据迁移指南](migrating-to-v2)

?> Linux 和 Steam Deck 用户：请参阅 [Linux 安装指南](installing-r2modman-linux)

?> Mac用户请参阅 Candygoblen123的 [Trombone Champ Mod Manager for Mac](https://github.com/Candygoblen123/TromboneChampModManager/)

?> 安装TootTally的游戏内自制歌曲下载器的视频指南，见 [Rayanne的教程视频](https://youtu.be/p0rud1uJ0o0?si=sDlmbDg3geAEW5J3) 游戏内歌曲下载器的相关内容请参阅 [安装歌曲](installing-songs)

本指南将讲解如何安装并使用 [r2modman](https://github.com/ebkr/r2modmanPlus/releases/latest/) 来下载和运行 [Thunderstore](https://trombone-champ.thunderstore.io/) 上的可用的模组。 使用像 r2modman 这样的模组管理器可以让您轻松更新和使用最新版本的模组，因为管理器会为您完成所有这些工作！ 本指南中我们以安装 **TrombLoader**为例，安装其他mod的方式与之相同。

## 安装 r2modman

?> 最新版本的 r2modman 是 **%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b}**

首先从Github上下载r2modman，点击→[**R2modman GitHub page**](https://github.com/ebkr/r2modmanPlus/releases/latest/).

**Windows用户**应该下载 [`r2modman-Setup-%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b}.exe`](https://github.com/ebkr/r2modmanPlus/releases/download/v%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b:raw}/r2modman-Setup-%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b:raw}.exe) 或 [`r2modman-%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b}.exe`](https://github.com/ebkr/r2modmanPlus/releases/download/v%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b:raw}/r2modman-%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b:raw}.exe)。 前者将模组管理器安装到你的系统中，而后者会直接运行 r2modman，无需任何安装。 只需运行安装包或程序即可打开 r2modman。

要下载，只需单击如下所示的链接并运行你刚刚下载的程序。

![r2modman GitHub Download (v3.1.39)](../docs/files/r2modman-install/r2modmandownload.png)

## 使用 r2modman 安装模组

成功安装 r2modman 后，你终于可以安装模组了。

1. 启动 **r2modman** 你将看到以下界面。

![r2modman游戏选择界面](../docs/files/r2modman-install/gameselection.png)

2. 选择 **"Trombone Champ"**, 然后点击 **"Select Game"**.

?> 如果列表中没有Trombone Champ, **使用搜索栏或使用鼠标滚轮向下滚动** 来找到 "Trombone Champ".

![选择Trombone Champ](../docs/files/r2modman-install/selecttc.png)

3. 它会要求你选择要使用的配置文件。 在本指南中，我们将使用默认配置文件。 单击 **Select profile**。

![选择Default Profile](../docs/files/r2modman-install/profileselect.png)

4. 这将引导我们进入此画面。

![首次打开](../docs/files/r2modman-install/firsttimeinstall.png)

5. 点击侧边栏上的 **“Online”**。 会出现一个所有可在 [Thunderstore](https://trombone-champ.thunderstore.io/) 下载的模组的列表。

![点击 Online](../docs/files/r2modman-install/selectonline.png)

6. 从这里，你可以选择要下载和安装的模组。 点击 **TrombLoader**，然后单击“Download”。

?> 如果您没有找到 **TrombLoader**, 可以使用搜索栏或使用鼠标滚轮向下滚动.

![下载TrombLoader](../docs/files/r2modman-install/downloadtrombloader.png)

7. 它会询问你要使用哪个版本。 下载最新版本，默认情况下已为你选择该版本。 点击 **"Download with dependencies"** 请注意，此操作也会下载Trombloader的所有前置模组，这些模组是Trombloader正常运行的必要组件。

![下载必要前置文件](../docs/files/r2modman-install/downloadlatest.png)

8. 安装好模组后，你可以单击侧边栏上的“Start modded”。 这将启动已安装模组后的游戏。

![启动Trombone Champ Modded](../docs/files/r2modman-install/startmodded.png)

大功告成！ 你刚刚成功为长号冠军安装了模组！ 下一步是 [安装自制谱面](installing-songs)

祝你玩得开心，长号冠军！

