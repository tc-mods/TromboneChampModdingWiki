# 在 Linux 和 Steam Deck上使用 r2modman
---

?> 本指南中我们以安装 **TrombLoader**为例，安装其他mod的方式与之相同 。

本指南将讲解如何安装并使用 [r2modman](https://github.com/ebkr/r2modmanPlus/releases/latest/) 来下载和运行 [Thunderstore](https://trombone-champ.thunderstore.io/) 上的可用的模组。 使用像 r2modman 这样的模组管理器可以让您轻松更新和使用最新版本的模组，因为管理器会为您完成所有这些工作！（译者注：本人从未使用过linux，因此部分用词难免出现错误，敬请谅解。必要时请参考英文原文。）

## Steam Deck所需的前置准备
在继续使用本指南前，Steam Deck需要预先进行以下操作。

 - 确保游戏安装到内部存储中 - 如果游戏安装到MicroSD卡，模组将无法加载。
 - 按住电源按钮并从菜单中选择桌面模式以进入 **桌面模式**。

进入桌面模式之后，所需的准备就完成了！

!> r2modman **无法在游戏模式下运行**。 请参阅[**在Steam Deck游戏模式下使用模组**](installing-r2modman-linux?id=using-mods-in-steam-decks-game-mode)来获得解决办法，在**安装r2modman**完成之后。

## 安装 r2modman

?> 最新版本的 r2modman 是 **%{thunderstore:f21c391c-0bc5-431d-a233-95323b95e01b}**

对于 Linux，r2modman可根据发行版的不同而提供不同的软件包格式：

 - `deb` 提供给Debian与基于Ubuntu的发行版
 - `pacman` 提供给基于Arch的发行版
 - `rpm` 提供给使用RPM Package Manager (RHEL, CentOS, Fedora, openSUSE, etc.) 的发行版
 - `AppImage`, 大多数发行版都可用的版本 - **Steam Deck可用**

访问 [**r2modman GitHub 发布页面**](https://github.com/ebkr/r2modmanPlus/releases/latest/) 并下载您的发行版所对应的软件包文件并根据您的软件包管理器文档安装它。

**Steam Deck用户** 请下载 `.AppImage`并将其保存在安全的位置，例如桌面或者“文档”文件夹中。 您还需要将文件标记为可执行文件。 右键点击 `.AppImage` 文件并选择`Properties`。 切换到 **Permissions** 标签，然后勾选框标记 `Is Executable` 然后单击OK。

![Steam Deck Permissions窗口](../docs/files/r2modman-linux/appimageproperties.png)

在将文件标记为可执行文件后，您现在可以双击 `AppImage` 打开 r2modman。

## 使用 r2modman 安装模组

成功安装 r2modman 后，你终于可以安装模组了。

1. 启动 **r2modman** 你将看到以下界面。

![r2modman游戏选择界面](../docs/files/r2modman-linux/gameselection.png)

2. 选择 **"Trombone Champ"**, 然后点击 **"Select Game"**.

?> 如果列表中没有Trombone Champ, **使用搜索栏或使用鼠标滚轮向下滚动** 来找到 "Trombone Champ".

![选择Trombone Champ](../docs/files/r2modman-linux/selecttc.png)

3. 它会要求你选择要使用的配置文件。 在本指南中，我们将使用默认配置文件。 单击 **Select profile**。

![选择Default Profile](../docs/files/r2modman-linux/profileselect.png)

4. 这将引导我们进入此画面。

![首次打开](../docs/files/r2modman-linux/firsttimeinstall.png)

5. 点击侧边栏上的 **“Online”**。 会出现一个所有可在 [Thunderstore](https://trombone-champ.thunderstore.io/) 下载的模组的列表。

![点击 Online](../docs/files/r2modman-linux/selectonline.png)

6. 从这里，你可以选择要下载和安装的模组。 点击 **TrombLoader**，然后单击“Download”。

?> 如果您没有找到 **TrombLoader**, 可以使用搜索栏或使用鼠标滚轮向下滚动。

![下载TrombLoader](../docs/files/r2modman-linux/downloadtrombloader.png)

7. 它会询问你要使用哪个版本。 下载最新版本，默认情况下已为你选择该版本。 点击 **"Download with dependencies"** 或者**"Download"**。

![下载必要前置文件](../docs/files/r2modman-linux/downloadlatest.png)

8. 对 **"BepInExPack_TromboneChamp"**进行相同操作。

![正在下载 BepInExPack_TromboneChamp](../docs/files/r2modman-linux/downloadbepinex.png)

9. 安装好模组后，你可以单击侧边栏上的“Start modded”。 这将启动已安装模组后的游戏。

![启动Trombone Champ Modded](../docs/files/r2modman-linux/startmodded.png)

大功告成！ 你刚刚成功为长号冠军安装了模组！

祝你玩得开心，长号冠军！

## 使用 r2modman 安装自制谱面

安装自制谱面的步骤与[安装自制谱面](installing-songs)中给出的安装方式基本相同。 唯一的区别是您需要找到您的 `BepInEx` 文件夹。 可以通过单击r2modman侧边栏上的“Settings”，然后点击“Browse profile folder”来打开它。

![Browse profile folder](../docs/files/r2modman-linux/browseprofile.png)

由此, 您的 `BeepInEx` 文件夹就会出现。

![Profile Folder](../docs/files/r2modman-linux/profilefolder.png)

!> 如果您的 `BepInEx` 文件夹中没有 `CustomSongs` 文件夹， **点击Start Modded来运行一次游戏**。 如果文件夹没有正常生成，您也可以手动创建它。

自此，可继续按照 [安装自制谱面](installing-songs)教程中的划线部分进行操作。

## 让视频类谱面背景正常工作。
一些自制谱面可能包含视频文件，默认的Proton设置无法播放。 如果您想要这些视频文件正常播放，可以安装`GE-Proton`，使用[ProtonUp-Qt](https://davidotek.github.io/protonup-qt/)。 这是一个包含一些额外功能的Proton版本，包括能够播放Valve官方无法支持的视频格式。

我们建议查阅 [由 GamingOnLinux创建的指南](https://www.gamingonlinux.com/2022/03/protonup-qt-got-upgraded-heres-how-to-use-it-on-steam-deck-and-linux/) ，用于说明如何使用 ProtonUp-Qt 并安装 `GE-Proton`

！> 即便使用GE-Proton, 您仍然可能会遇到一些视频播放方面的问题，这取决于您的设置。

## 在Steam Deck游戏模式下使用模组
**r2modman无法在Steam Deck的游戏模式下运行, 因此模组文件不会被加载。** 想要解决这个问题，需要您在Steam中右键点击长号冠军并点击`属性Properties`。 将下面的内容复制进**启动选项Launch Options**中:

```
WINEDLLOVERRIDES="winhttp=n,b" %command% --doorstop-enable true --doorstop-target "/home/deck/.config/r2modmanPlus-local/TromboneChamp/profiles/Default/BepInEx/core/BepInEx.Preloader.dll" --r2profile "Default"
```
![Steam属性](../docs/files/r2modman-linux/steamproperties.png) 这将指示游戏使用我们早些时候在 r2modman 中配置的默认配置文件启动，您安装的所有模组和自定义歌曲都可以正常使用。
