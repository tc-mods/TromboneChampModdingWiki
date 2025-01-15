# 安装自制谱面（Meta Quest篇）

---

!> **注意：** 本篇教学适用于**Meta Quest**上的VR游戏——_长号冠军：Unflattened_。 如果要为**Steam**版本安装自制谱面，请参阅 [此教学](installing-songs-steamvr)。<br><br>要为PC本作安装自制谱面，请参阅 [长号冠军模组安装教学](installing-r2modman)。

长号冠军：Unflattened 内置自制谱面支援，并与本作的谱面相容。 游戏仅支援视频和图像背景，无法使用在Unity制作的自制背景。

?> 你可以在 [TootTally](https://toottally.com/) 或 [TromboneDB](https://tc-mods.github.io/TromboneDB/)找到社区制作的谱面。

## 通过 USB 添加谱面

1. 解压缩包含您准备复制谱面的ZIP文件。 请确保每个谱面各自的文件夹中都包括的所需的文件(`song.ogg`、`song.tmb`、`bg.png`或`bg.mp4`)。

![从ZIP文件中解压缩谱面](../docs/files/vr/questextract.png)

2. 使用 USB 线连接您的VR头显到您的电脑。 你应该看到你的头显在电脑上显示为removable storage（可移动存储设备）。

![Meta Quest 3 通过 USB 连接到 Windows](../docs/files/vr/questusbconnected.png)

?> macOS 用户需要使用第三方应用程序（如 [OpenMTP](https://openmtp.ganeshrvel.com)）来访问他们Quest的存储空间。

3. 打开Quest的内部存储，然后导航到 `/Android/data/com.ImpactReality.TromboneChamp/files/customtracks/`。 拖放您早些时候创建的谱面文件夹到 `customtracks` 中。

![拖拽谱面到Quest中](../docs/files/vr/questdraganddrop.png)

4. 一旦您完成了复制您想要的歌曲，开始游戏， 选择 **Free Play**，然后你会发现你的自制谱面列在它们的独立类别中。

![在游戏中显示的自定义歌曲](../docs/files/vr/ingamequest.png)

## 搜索自制谱面

您可以在许多地方找到长号冠军的自制谱面。 以下是几个选项：

- [TootTally网站](https://toottally.com/search/)上的搜索功能。
- [TromboneDB](https://tc-mods.github.io/TromboneDB/)是一个拥有大部分已发布谱面的档案库，包括对于Tootally来说过大的谱面。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 `#custom-charts` 频道。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 Tootbender 机器人谱面搜索命令。
- 大多数自制谱面在Youtube上都有演示视频。 部分视频会在描述中包含下载链接。

### 制作谱面 {docsify-ignore}

> 参阅此[**写谱教程**](creating-charts)以了解如何制作您自己的谱面。
