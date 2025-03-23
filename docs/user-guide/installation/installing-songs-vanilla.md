# Installing Songs (Vanilla)
---

!> **NOTE:** It is still **highly recommended** to [install songs using mods](installing-songs)! This allows you to download charts straight from your game without having to open up a web browser and having to download them to specific folders!

As of Trombone Champ version 1.25, the non-modded (vanilla) game can now play custom charts that the community has created! This is done in-game through the use of "Custom Track Collections", a special folder where the game looks for custom charts that it can read and play for you. This guide will show you how to use this new feature!

## Finding the Custom Track Collections Folder

You can find this folder by peeking into Settings > Custom Track Collections.

![Settings Screen](../docs/files/vanilla/settingscreen.png)

![Custom Tracks and Collections Screen](../docs/files/vanilla/customtracks.png)

?> **NOTE:** By default, this folder will be located inside your Trombone Champ's installation location at `<TromboneChampLocation>/TromboneChamp_Data/StreamingAssets/custom_track_collections`

![Browse Local Files](../docs/files/localfilescontext.png)

![Trombone Champ Installation Location](../docs/files/vanilla/tcinstalllocation.png)

![Trombone Champ Data Folder](../docs/files/vanilla/tcdata.png)

![Trombone Champ StreamingAssets Folder](../docs/files/vanilla/tcstreamingassets.png)

![Trombone Champ Custom Collections Folder](../docs/files/vanilla/tccollections.png)

## Creating a New Collection

To create a new collection:

1. Create a folder. Name it whatever you would like this collection to be called.

2. Inside this folder, create a file named `collection_metadata.json`. Make sure that this isn't named `collection_metadata.json.txt`.

3. Inside the `collection_metadata.json` file, write down the following:

    ```json
    {
      "name":"Write down the title of your collection here.",
      "description":"Describe what this collection is for in this text."
    }
    ```

?> **NOTE:** You can always peek at the `sample_collection_folder` to figure out what a collection folder should look like.

## Finding Charts

?> **NOTE:** This section is a line-by-line copy from the main [Song Installation Guide](installing-songs?id=finding-songs).

There are a number of places you can find Trombone Champ custom songs online. Here are a few options:

- TootTally's in-game song downloader. Note that not all charts may be available for download in-game.
- The search function on the [TootTally website](https://toottally.com/search/). Any results you get here will likely be the same as what the in-game song downloader would have.
- [TromboneDB](https://tc-mods.github.io/TromboneDB/) has an archive of the majority of charts released, including charts that are too large for TootTally.
- The `#custom-charts` channel in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- The Tootbender bot's chart search command in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- Most charts have showcase videos on YouTube. Sometimes they will have download links in the description.

## Placing Your Downloaded Charts

Now that you have downloaded some charts, it's time to place them into your folder! Simply drag and drop the **UNZIPPED** folders inside the folder you created. It should look like the following.

![Wiki Collections Folder](../docs/files/vanilla/collectiondemonstration.png)

## Playing Your Custom Charts

Once you have compiled all your charts, open the game and go into the song selection screen. You should see a box at the bottom right that shows which collection you're viewing. By default, this is the "Trombone Champ Collection" which are all the songs that come with the game.

![Song List](../docs/files/vanilla/songlist.png)

Click that collections button and find your collection.

![Collections Selection](../docs/files/vanilla/collectionselection.png)

Click OK and verify that your charts are all in there.

![Collection Tracks](../docs/files/vanilla/collectionview.png)

And that should be it! Happy tooting!
