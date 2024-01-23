谱面制作常见问题
---

在制作自制谱面时遇到了问题？ 可以在这里寻找答案！

### 我的谱面无法在长号冠军里正常运行！ 我可以控制长号，但我无法暂停。

这类问题通常与您的 `song.ogg` 文件有关。 请确保您正确放置 `song.ogg`文件，并且它的曲目时长要超过谱面文件的时长（取决于谱面的结束点 endpoint）。 如有必要，可以在 `song.ogg` 末尾额外添加几秒静音来将其延长。

### 我的谱面在末尾或在中途会出现卡死，并且无法暂停。但我仍然可以控制长号。

解决方法同上（我的谱面无法在长号冠军里正常运行！）

### 在我点击某个特定音符时，长号冠军出现了卡顿甚至卡死。当曲目结束时我被莫名其妙扣掉了30亿toots？？ （或者Autotoot模式下出现了F或者0分）

这可能是由于在谱面卡顿的地方隐藏了一个幽灵音符。 Check your MIDI file for a note hiding under the note you want in the chart, or check that spot for something funky in Trombone Charter/BonerViewer. Sometimes it will show up in one program but not another. Play the broken chart again and you can get your toots back. In old versions of Trombone Champ, this was similar to an issue with tap notes. Check if you're up to date!

### Certain spots in my chart always break combo, even when Autotoot plays it

Check for ghost notes hiding under your main notes in those spots! Check your MIDI, Trombone Charter, and/or BonerViewer. They may show up with one program but not another. Remember that autotoot isn't perfect. You can change some of the settings in its config file to try to make it more accurate, but sometimes it just can't keep up with very fast notes.

### My chart doesn't show up in the track list

Ensure that your chart has a unique `trackref`. Open the tmb file with notepad, press Ctrl+F, and search for `trackref`. If the `trackref` value is something not unique (e.g. `trombonecharter_x64` or a common song name), change it to something that won't be confused with another chart. If you are concerned that you may have multiple charts installed with duplicate trackrefs, you can try running [Guardie's trackref duplicate finder](https://github.com/Guarde/TrackRef-Checker/releases/latest) in your customsongs folder.

### My chart background is small and has a gray border around it

Ensure that your background has dimensions of 1920 x 1080.

### My chart background doesn't show up at all

Ensure that your background is named `bg.png` (if it's an image), `bg.mp4` (if it's a video), or `bg.trombackground` (if it's a TromBackground)

### I'm still having problems

If you are still having problems, you may want to consider asking for help in the Trombone Champ Modding Discord server. Be prepared to send the `LogOutput.log` file from your BepInEx folder so we can take a look at what happened when the game broke.
