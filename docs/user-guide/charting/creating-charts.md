# Creating Charts
---

?> If you prefer video tutorials, NyxTheShield has [a stream archive](https://www.youtube.com/watch?v=ig27SlJveGs) that explains every step of the charting process in detail.

## Basics
### Midi Editor/DAW
Charts are made by creating a midi file and running them through a [MIDI converter](#converting-midi-to-map-file).

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

Some free, verified to work midi editors include:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*Full software is not free, but has a free trial that works for charting.</sub><br>
<sub>**Exports notes into MIDI track 2 by default, which makes it incompatible with Midi2TromboneChamp by default.</sub><br>
<sub>†The trial version of FL Studio doesn't allow you to export MIDI, but you can get around this by saving the project file and using [flp2midi](https://github.com/Kaydax/flp2midi/releases/latest).

#### Reaper Project
If you're not sure which editor to use, Reaper is recommended as there's a custom Trombone Champ project file that comes with:
- A basic explanation on how to use the controls of Reaper (in English)
- Preconfigured settings
- Example MIDI

The project can be [downloaded here](https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip).

### Normal Notes

Normal notes are created in the midi editor and look the same in-game. Make sure to leave a gap in time between notes!

### Slide Notes

Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.

![Slide Note Example](../docs/files/slide1.png)

To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.

![Multiple Slide Note Example](../docs/files/slide2.png)

## Converting Midi to Map File

1. Go to [Trombone Champ Chart Converter](https://tc-chart-converter.github.io/).

2. Fill out the fields:
 - `Song Name` is the full name of the song, shown in the info when you select it in-game.
 - `Short Name` is shown while scrolling through the song list.
 - `Artist` is the composer of the song.
 - `Release Year` is the year the song was created.
 - `Beats per Bar` determines how far apart the "beat lines" are.
 - `Difficulty` is the number of difficulty stars that appear on the song's info.
 - `Note Spacing` affects how fast the level scrolls, in combination with BPM.
 - `trackRef` is the globally unique name used by mods to identify your chart.
 - `Song Endpoint` is the beat on which the song ends. It is automatically calculated, but you can adjust it to change when the level end screen appears.

4. Hit OK. Create a folder with the same name as you entered in the `trackRef` field, and save the file as `song.tmb` inside that folder.

5. Your music track should be a .ogg file. You can use software like Audacity to insert silence at the start of the track to line it up with the midi. Name the file `song.ogg`.

6. Move the ogg file into the same folder as `song.tmb`.

7. Follow the [Custom Song Installation instructions](installing-songs) to test it.

8. [Add a background!](chart-backgrounds)
