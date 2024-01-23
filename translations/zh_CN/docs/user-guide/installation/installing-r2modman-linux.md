# 在 Linux 和 Steam Deck上使用 r2modman
---

?> 本指南中我们以安装 **TrombLoader**为例，安装其他mod的方式与之相同 。

本指南将讲解如何安装并使用 [r2modman](https://github.com/ebkr/r2modmanPlus/releases/latest/) 来下载和运行 [Thunderstore](https://trombone-champ.thunderstore.io/) 上的可用的模组。 使用像 r2modman 这样的模组管理器可以让您轻松更新和使用最新版本的模组，因为管理器会为您完成所有这些工作！

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

**For Steam Deck users,** download the `.AppImage` file and keep it in a safe location such as your Desktop or your Documents folder. You will also need to mark the file as executable. To do this, right-click the `.AppImage` file and select `Properties`. Switch to the **Permissions** tab and check the box marked `Is Executable` and click OK.

![Steam Deck Permissions Window](../docs/files/r2modman-linux/appimageproperties.png)

After marking the file as executable, you can now double-click the `AppImage` to open r2modman.

## Installing Mods on r2modman

Once you have succesfully installed r2modman, you can finally install mods.

1. Launch **r2modman**. You will be greeted with the following screen.

![r2modman Game Selection Screen](../docs/files/r2modman-linux/gameselection.png)

2. Select **"Trombone Champ"**, and click **"Select Game"**.

?> If you do not see it, **use the search bar or scroll down** to find "Trombone Champ".

![Select Trombone Champ](../docs/files/r2modman-linux/selecttc.png)

3. It will ask you to choose which profile to use. For this guide's purposes, we will stick with the Default profile. Click **"Select profile"**.

![Select Default Profile](../docs/files/r2modman-linux/profileselect.png)

4. This will lead us to this screen.

![First Time Opening Installed](../docs/files/r2modman-linux/firsttimeinstall.png)

5. Click **"Online"** on the sidebar. This will bring up a list of all available to download mods on [Thunderstore](https://trombone-champ.thunderstore.io/).

![Clicking Online](../docs/files/r2modman-linux/selectonline.png)

6. From here, you may choose which mods you would like to download and install. Click on **TrombLoader**, and then click on Download.

?> If you do not see **TrombLoader**, use the search bar or scroll down.

![Downloading TrombLoader](../docs/files/r2modman-linux/downloadtrombloader.png)

7. It will ask you which version to use. Download the latest version, which is already selected for you by default. Click **"Download with dependencies"** or **"Download"**.

![Downloading with dependencies](../docs/files/r2modman-linux/downloadlatest.png)

8. Do the same for **"BepInExPack_TromboneChamp"**.

![Downloading BepInExPack_TromboneChamp](../docs/files/r2modman-linux/downloadbepinex.png)

9. Once you are done installing your mods, you may click on "Start modded" on the sidebar. This will launch the game with your mods.

![Start Trombone Champ Modded](../docs/files/r2modman-linux/startmodded.png)

That's it! You have just successfully modded Trombone Champ!

Godspeed, Tromboner.

## Installing Custom Songs on r2modman

The steps for installing custom songs are more or the less the same as specified in the [Installing Songs](installing-songs) guide. The only difference is that you need to find your `BepInEx` folder. It can be found by clicking "Settings" on the sidebar, and then clicking on "Browse profile folder".

![Browse profile folder](../docs/files/r2modman-linux/browseprofile.png)

From there, your `BepInEx` folder is the `BepInEx` folder that you see.

![Profile Folder](../docs/files/r2modman-linux/profilefolder.png)

!> If there is no `CustomSongs` folder inside your `BepInEx` folder, **run the game once by clicking Start Modded**. If that doesn't generate the folder, you may make it yourself.

From there, follow the steps outlined in the [Installing Songs](installing-songs) guide.

## Getting Video Backgrounds Working
Some custom songs will include videos for their backgrounds, and the default Proton install cannot play these back. If you want these to work, you can install `GE-Proton` using [ProtonUp-Qt](https://davidotek.github.io/protonup-qt/). This is a version of Proton that includes some additional features, including the ability to play back video formats that Valve are unable to support officially.

We recommend following [this guide created by GamingOnLinux](https://www.gamingonlinux.com/2022/03/protonup-qt-got-upgraded-heres-how-to-use-it-on-steam-deck-and-linux/) for instructions on how to use ProtonUp-Qt and install `GE-Proton`.

!> Even with GE-Proton, you may still experience some issues with video playback depending on your setup.

## Using Mods in Steam Deck's Game Mode
**r2modman will not work in Steam Deck's Game mode, and therefore mods will not load by default.** To get around this, right-click the game in Steam and click `Properties`. From there, paste the following into **Launch Options**:

```
WINEDLLOVERRIDES="winhttp=n,b" %command% --doorstop-enable true --doorstop-target "/home/deck/.config/r2modmanPlus-local/TromboneChamp/profiles/Default/BepInEx/core/BepInEx.Preloader.dll" --r2profile "Default"
```
![Steam Properties](../docs/files/r2modman-linux/steamproperties.png) This will instruct the game to launch with the Default profile we configured in r2modman earlier, so all your mods and custom songs installed there will be available.
