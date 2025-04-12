# Installing Songs (Vanilla)

---

!> **注意:** 仍然**强烈推荐**[使用mods安装歌曲](installing-songs)！ 安装mod允许您直接在游戏内搜索、下载并直接游玩谱面，而无需打开网页浏览器并将它们下载到指定的文件夹！

长号冠军Trombone Champ更新至1.25版本之后，游戏现在可以在不依靠任何mod的情况下（原生）游玩由社区内玩家制作的自制谱面！ 通过将自制谱面文件放入特定的文件夹中，并使用游戏中的“自定义曲目收藏”功能，就可以像安装了mod一样游玩自制谱面。 本指南将向您介绍如何使用这个新功能！

## 查找自定义曲目文件夹

您可以在设置 > 自定义曲目与合集中找到此文件夹。

![“设置”界面](../docs/files/vanilla/settingscreen.png)

![“自定义曲目与合集”界面](../docs/files/vanilla/customtracks.png)

?> **注意:** 默认情况下，这个文件夹在您长号冠军Trombone Champ的安装位置中，位于`<TromboneChampLocation>/TromboneChamp_Data/StreamingAssets/custom_track_collections`

![Browse Local Files](../docs/files/localfilescontext.png)

![Trombone Champ Installation Location](../docs/files/vanilla/tcinstalllocation.png)

![Trombone Champ Data Folder](../docs/files/vanilla/tcdata.png)

![Trombone Champ StreamingAssets Folder](../docs/files/vanilla/tcstreamingassets.png)

![Trombone Champ Custom Collections Folder](../docs/files/vanilla/tccollections.png)

## 创建一个新的合集

To create a new collection:

1. Create a folder. 这个文件夹的名字将作为该“合集”的名称。

2. Inside this folder, create a file named `collection_metadata.json`. 请确保删除 `.txt`，以`.json`为文件后缀。

3. Inside the `collection_metadata.json` file, write down the following:

        {
          "name":"Write down the title of your collection here.",
          "description":"Describe what this collection is for in this text."
        }

?> **注意:** 你可以随时以 `sample_collection_folder`文件夹作为合集文件夹的创建参考 。

## 获取谱面

?> **注意:** 本节内容完全复制自[安装自制谱面](installing-songs?id=finding-songs)中的相同小节。

您可以在许多地方找到长号冠军的自制谱面。 以下是几个选项：

- 游戏内的TootTally Song Downloader歌曲下载器（mod）。 请注意并非所有谱面都可以在游戏中下载。
- [TootTally网站](https://toottally.com/search/)上的搜索功能。 您在这里得到的任何结果都可能与游戏内的歌曲下载器相同。
- [TromboneDB](https://tc-mods.github.io/TromboneDB/)是一个拥有大部分已发布谱面的档案库，包括对于Tootally来说过大的谱面。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 `#custom-charts` 频道。
- [Discord长号冠军模组群](https://discord.gg/KVzKRsbetJ)中的 Tootbender 机器人谱面搜索命令。
- 大多数自制谱面在Youtube上都有演示视频。 部分视频会在描述中包含下载链接。

## 将你下载的自制谱放入游戏中

现在你已经下载了一些自制谱，现在是把它们放到你的文件夹中的时候了！ 只需将 **已解压** 的自制谱文件夹放入你创建的合集文件夹中。 放入之后应该如下图所示。

![Wiki合集文件夹](../docs/files/vanilla/collectiondemonstration.png)

## 游玩您下载的自制谱面

放置好您下载的自制谱面之后，打开游戏并进入选择曲目界面。 You should see a box at the bottom right that shows which collection you're viewing. By default, this is the "Trombone Champ Collection" which are all the songs that come with the game.

![Song List](../docs/files/vanilla/songlist.png)

Click that collections button and find your collection.

![Collections Selection](../docs/files/vanilla/collectionselection.png)

Click OK and verify that your charts are all in there.

![Collection Tracks](../docs/files/vanilla/collectionview.png)

And that should be it! Happy tooting!
