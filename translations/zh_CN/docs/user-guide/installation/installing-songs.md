# 安装自制谱面
---
!> **注意：** 请确保您已经按照 [mod安装指南](installing-r2modman) 安装r2modman和 TrombLoader，然后再继续！

目前有两种方法来安装自制歌曲: TootTally游戏内的歌曲下载器或手动安装自制歌曲。 两种方法都会涵盖在本指南内！

## 游戏内的歌曲下载器 (推荐方法)

TootTally团队通过创建游戏内歌曲下载模组为Trombone Champ模组社区做出了重大的贡献。 通过这个模组下载的所有谱面都来自TootTally的服务器，其中包含了社区中绝大多数谱面的文件。 要安装和使用游戏内的歌曲下载器。请：

1. 打开 r2modman，然后点击Online标签页显示可用的模组。 ![点击 Online](../docs/files/r2modman-install/selectonline.png)

2. 在搜索栏中搜索 `song downloader`。 找到之后选择它，点击"Download"然后点击 "Download with dependencies" ，就像安装其他模组那样。 ![寻找歌曲下载器](../docs/files/songdownloader/findingsongdownloader.jpg)

3. 点击"Start Modded." 长号冠军将会启动。 ![启动Trombone Champ Modded](../docs/files/r2modman-install/startmodded.png)

4. 选择你的存档并开始游戏。 在主菜单界面，点击左边的"Mod Settings"按钮。 ![Mod 设置](../docs/files/songdownloader/modsettings.jpg)

5. 点击"More Songs"按钮。 ![更多歌曲](../docs/files/songdownloader/moresongs.jpg)

6. 点击“SearchHere”并输入您想要下载的歌曲名称。 点击回车进行搜索。 ![搜索](../docs/files/songdownloader/search.jpg)

7. 如果该歌曲的谱面存在并可下载，请点击download按钮。 ![Song Downloader](../docs/files/songdownloader/songdownload.jpg)

大功告成！ 您可以像游玩游戏内置谱面一样游玩这些自制谱面了。

当你搜索到你想要的曲子时，可能会有一个N/A标志取代download按钮。 它的意思是该歌曲的谱面存在，但您不能通过游戏内的歌曲下载器下载。 您仍然可以手动安装该谱面！

## 手动安装谱面

?> 视频教程请参阅 [Rayanne's guide on installing custom songs manually](https://www.youtube.com/watch?v=p0rud1uJ0o0).

1. 单击r2modman侧边栏上的“Settings”，然后点击“Browse profile folder”。

![Browse profile folder](../docs/files/r2modman-install/browseprofile.png)

2. 点击 `BepInEx` 文件夹。

![Profile Folder](../docs/files/r2modman-install/profilefolder.png)

3. `CustomSongs` 文件夹是游戏存储所有自制谱面文件的地方。 点击文件管理器窗口上方的地址栏以显示该文件夹的地址，并复制地址栏中的内容。

![BeepInEx 文件夹](../docs/files/r2modman-install/bepinexfolder.png)

!> 如果您的 `BepInEx` 文件夹中没有 `CustomSongs` 文件夹， **点击Start Modded来运行一次游戏**。 如果文件夹没有正常生成，您也可以手动创建它。

4. 下载自制谱面。通常情况下是一个压缩包，以`.zip`等压缩包格式作为文件名结尾。 搜索自制谱面可参阅本页末尾。

6. 解压压缩包内的全部内容并放入 `BepInEx/CustomSongs`文件夹。 您可以通过右键点击压缩包并点击“解压缩全部”，将之前复制的文件夹地址放入目标地址栏。

![BeepInEx 解压缩预览](../docs/files/customsongextract.png)

7. 请仔细检查歌曲是否在存储在它自己的文件夹，而不是直接在 CustomSongs 文件夹中的散装文件。 同时也请确认自制谱面的全部文件只在一个文件夹中，而不是嵌套在多个文件夹中—— 举一个例子， 所有的文件都应该位于 `BepinEx/CustomSongs/BakaMitai`文件夹内。

![正确解压缩预览](../docs/files/customsongcorrect.png)

## 搜索自制谱面

您可以在许多地方找到长号冠军的自制谱面。 以下是几个选项：
- TootTally的游戏内歌曲下载器。 请注意并非所有谱面都可以在游戏中下载。
- [TootTall网站](https://toottally.com/search/) 上的搜索功能。 您在这里得到的任何结果都可能与游戏内的歌曲下载器相同。
- 在`#custom-charts` 频道中找到，请至[Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ)。
- [Trombone Champing Discord](https://discord.gg/KVzKRsbetJ)中的Tootbender 机器人谱面搜索命令。
- ~~TheGlitched64's [spreadsheet containing information on every custom chart](https://docs.google.com/spreadsheets/d/1xpoUnHdSJFqOQEK_637-HCECYtJsgK91oY4dRuDMtik/edit?usp=sharing).~~
  - Discord has since disabled the ability to link files externally, so most links in the spreadsheet will no longer work. We have created [TromboneDB](https://tc-mods.github.io/TromboneDB/) as a replacement which has download mirrors for all charts.
- 大多数自制谱面在Youtube上都有演示视频。 有时，它们会在视频描述中包含下载链接。

### 制作自制谱面 {docsify-ignore}

> 请参考[**Charting guide**](creating-charts) 来获取制作自制谱面的信息！
