# Installing Songs (Meta Quest Version)
---
!> **IMPORTANT:** This guide is for the VR game *Trombone Champ: Unflattened* on **Meta Quest**. For installing custom songs in the **Steam** version, check [this guide](installing-songs-steamvr).<br><br>For installing custom songs in the standard game, see the [mod installation guide for Trombone Champ](installing-r2modman).

Trombone Champ: Unflattened has built-in custom song support, and is compatible with charts made for the standard game. Do note that only video and image backgrounds will work, custom backgrounds made in Unity will not.

?> You can find community made custom charts on [TootTally](https://toottally.com/), or by browsing [TromboneDB](https://tc-mods.github.io/TromboneDB/).

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

## Adding charts via SideQuest
idk lol

## Finding Songs

There are a number of places you can find Trombone Champ custom songs online. Here are a few options:
- The search function on the [TootTally website](https://toottally.com/search/).
- [TromboneDB](https://tc-mods.github.io/TromboneDB/) has an archive of the majority of charts released, including charts that are too large for TootTally.
- The `#custom-charts` channel in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- The Tootbender bot's chart search command in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- Most charts have showcase videos on YouTube. Sometimes they will have download links in the description.

### Creating Custom Songs {docsify-ignore}

> Check out the [**Charting guide**](creating-charts) for info on creating your own custom charts.
