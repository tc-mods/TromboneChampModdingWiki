# 安装自制谱面（Meta Quest篇）

---

!> **注意：** 本篇教学适用于**Meta Quest**上的VR游戏——_长号冠军：Unflattened_。 如果要为**Steam**版本安装自制谱面，请参阅 [此教学](installing-songs-steamvr)。<br><br>要为PC本作安装自制谱面，请参阅 [长号冠军模组安装教学](installing-r2modman)。

长号冠军：Unflattened 内置自制谱面支援，并与本作的谱面相容。 游戏仅支援视频和图像背景，无法使用在Unity制作的自制背景。

?> 你可以在 [TootTally](https://toottally.com/) 或 [TromboneDB](https://tc-mods.github.io/TromboneDB/)找到社区制作的谱面。

## Adding charts via USB

1. Extract the ZIP files containing the charts you want to copy over. Make sure each the files of each chart (the `song.ogg`, `song.tmb`, and `bg.png`/`bg.mp4`) are stored together in their own folder.

![Extracting a chart from a ZIP file](../docs/files/vr/questextract.png)

2. Connect your headset to your PC using a USB cable. You should see your headset appear as removable storage.

![Meta Quest 3 connected to Windows via USB](../docs/files/vr/questusbconnected.png)

?> macOS users will need to use a third-party application (such as [OpenMTP](https://openmtp.ganeshrvel.com)) in order to access the storage of their Quest.

3. Open up the Quest's internal storage, and then navigate to `/Android/data/com.ImpactReality.TromboneChamp/files/customtracks/`. Drag and drop the chart folders you created earlier into `customtracks`.

![Drag and dropping the charts to the Quest](../docs/files/vr/questdraganddrop.png)

4. Once you've finished copying over the songs you want, start up the game, head into **Free Play**, and then you'll find your custom songs listed in their own category.

![Custom song shown in-game](../docs/files/vr/ingamequest.png)

## 搜索自制谱面

您可以在许多地方找到长号冠军的自制谱面。 以下是几个选项：

- [TootTally网站](https://toottally.com/search/)上的搜索功能。
- [TromboneDB](https://tc-mods.github.io/TromboneDB/)是一个拥有大部分已发布谱面的档案库，包括对于Tootally来说过大的谱面。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 `#custom-charts` 频道。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 Tootbender 机器人谱面搜索命令。
- 大多数自制谱面在Youtube上都有演示视频。 部分视频会在描述中包含下载链接。

### 制作谱面 {docsify-ignore}

> 参阅此[**写谱教程**](creating-charts)以了解如何制作您自己的谱面。
