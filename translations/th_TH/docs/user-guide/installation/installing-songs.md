# การลงเพลงที่กำหนดเอง
---
!> **IMPORTANT:** Make sure you've followed the [mod installation guide](installing-r2modman) to install r2modman and Trombloader before continuing!

There are currently two methods to installing custom songs: TootTally's in-game song downloader or installing custom songs manually. Both methods will be covered here!

## In-Game Song Downloader (Recommended Method)

The TootTally team has done the Trombone Champ Modding community a huge favour by creating the in-game song downloader mod. All charts downloaded by this mod come from TootTally's server, which holds mirrors of most charts. To install and use the in-game song downloader:

1. Open r2modman and click on the Online tab to show available mods. ![Clicking Online](../docs/files/r2modman-install/selectonline.png)

2. In the search bar, search for `song downloader`. Once you find it, select it, then click "Download" and then "Download with dependencies" as you would for any other mod. ![Finding Song Downloader](../docs/files/songdownloader/findingsongdownloader.jpg)

3. Click "Start Modded." Trombone Champ will start up. ![Start Trombone Champ Modded](../docs/files/r2modman-install/startmodded.png)

4. Select your profile and start the game. On the main menu, click the "Mod Settings" button on the left. ![Mod Settings](../docs/files/songdownloader/modsettings.jpg)

5. Click the "More Songs" button. ![More Songs](../docs/files/songdownloader/moresongs.jpg)

6. Click on the "SearchHere" field and type the name of the song you want to download. Hit Enter to search. ![Search](../docs/files/songdownloader/search.jpg)

7. If a chart for that song exists and is available to download, hit the download button. ![Song Download](../docs/files/songdownloader/songdownload.jpg)

That's all there is to it! You can play custom charts the same way you play base game charts.

Now, you may have run into an issue where your song came up, but instead of a download button it said "N/A". In this case, the chart for that song exists but you can't download it through the in-game song downloader. You might still be able to install that chart manually though!

## Installing Songs Manually

?> For a video guide, see [Rayanne's guide on installing custom songs manually](https://www.youtube.com/watch?v=p0rud1uJ0o0).

1. In r2modman, click "Settings" on the sidebar, and then click on "Browse profile folder".

![Browse profile folder](../docs/files/r2modman-install/browseprofile.png)

2. From there, click on the `BepInEx` folder.

![Profile Folder](../docs/files/r2modman-install/profilefolder.png)

3. The `CustomSongs` folder is where the game stores all of your custom charts. From here, click on the address bar at the top of the file explorer window and copy it with Ctrl+C or by right clicking and clicking "Copy".

![BepInEx Folder](../docs/files/r2modman-install/bepinexfolder.png)

!> If there is no `CustomSongs` folder inside your `BepInEx` folder, **run the game once by clicking Start Modded**. If that doesn't generate the folder, you may make it yourself.

4. Download the new custom song - it will generally be some kind of archive file, usually ending in `.zip`. There is a section with info on where you can find charts at the bottom of this page.

6. Extract the contents of the archive file directly into the `BepInEx/CustomSongs` folder in the r2modman profile directory. You can do this by right clicking the archive, clicking "Extract All" and then pasting the address you copied earlier into the field that pops up by using Ctrl+V or right clicking.

![ตัวอย่างการแตกไฟล์ BepInEx](../docs/files/customsongextract.png)

7. Double check that the song is in its own folder, instead of the files being directly in the CustomSongs folder. The files also should not be nested in multiple folders - in this example, all the song's files should be located in `BepinEx/CustomSongs/BakaMitai/`.

![ตัวอย่างการแตกไฟล์ที่ถูกต้อง](../docs/files/customsongcorrect.png)

## การหาเพลง

There are a number of places you can find Trombone Champ custom songs online. Here are a few options:
- TootTally's in-game song downloader. Note that not all charts may be available for download in-game.
- The search function on the [TootTally website](https://toottally.com/search/). Any results you get here will likely be the same as what the in-game song downloader would have.
- The `#custom-charts` channel in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- The Tootbender bot's chart search command in the [Trombone Champ Modding Discord](https://discord.gg/KVzKRsbetJ).
- ~~TheGlitched64's [spreadsheet containing information on every custom chart](https://docs.google.com/spreadsheets/d/1xpoUnHdSJFqOQEK_637-HCECYtJsgK91oY4dRuDMtik/edit?usp=sharing).~~
  - Discord has since disabled the ability to link files externally, so most links in the spreadsheet will no longer work. We have created [TromboneDB](https://tc-mods.github.io/TromboneDB/) as a replacement which has download mirrors for all charts.
- Most charts have showcase videos on YouTube. Sometimes they will have download links in the description.

### การสร้างเพลงที่กำหนดเอง {docsify-ignore}

> ไปที่ [**คู่มือการสร้างผัง**](creating-charts) สำหรับการสร้างผังของคุณเอง
