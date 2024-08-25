# 长号冠军写谱教程
---

?> 如果您喜欢视频教程，NyxTheShield的 [直播回放](https://www.youtube.com/watch?v=ig27SlJveGs) 会详细解释自制谱过程的每一步。

## 基础
### Midi Editor/DAW
自制谱的制作需要创建Midi文件并使用[MIDI转换器](#converting-midi-to-map-file)进行转换。

Midi文件中的音符应该在47到73的范围内以匹配游戏内的音高范围。<br>**注意：**该范围在不同的编辑器上会对应不同的钢琴琴键范围。

一些免费可用的Midi编辑器包括：
- [Reaper](https://www.reaper.fm/download.php)* (琴键范围: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (琴键范围: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (琴键范围: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (琴键范围: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (琴键范围: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*完整版的软件并非免费，但只使用试用版依然可以完成谱面的制作。</sub><br> <sub>**默认情况下会导出到 Midi 轨道2，会导致无法使用Midi2TromboneChamp。</sub><br> <sub>†FL Studio的试用版无法直接输出Midi文件, 但你可以通过保存项目文件并使用 <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a>来解决这个问题.</p>

<h4 spaces-before="0">
  Reaper 项目文件
</h4>

<p spaces-before="0">
  如果您不确定使用哪个编辑器，推荐尝试Reaper。有一个使用Reaper制作的Trombone Champ自制文件示例，其中包括：
</p>

<ul>
  <li>
    关于如何使用Reaper的基础教程（英文）
  </li>
  <li>
    预设设置
  </li>
  <li>
    示例MIDI文件
  </li>
</ul>

<p spaces-before="0">
  这个项目可以在 <a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">这里</a>下载。
</p>

<h3 spaces-before="0">
  普通note
</h3>

<p spaces-before="0">
  普通的直线note可以直接在Midi编辑器中创建，并且在游戏中看起来是一样的。 请务必在note之间保留足够时间的空隙！
</p>

<h3 spaces-before="0">
  滑动note
</h3>

<p spaces-before="0">
  Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="滑动note示例" />
</p>

<p spaces-before="0">
  To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="长滑动note示例" />
</p>

<h2 spaces-before="0">
  转换Midi文件为谱面文件
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      使用<a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      填写谱面信息：
    </p>
    <ul>
      <li>
        <code>Song Name</code> 是歌曲的全名，当您在游戏中选择这个谱面时，这一条会显示在左上角。
      </li>
      <li>
        <code>Short Name</code> 该内容会显示在曲目滚动列表中.
      </li>
      <li>
        <code>Artist</code> 是歌曲的作曲家。
      </li>
      <li>
        <code>Release Year</code> 是歌曲发行的年份。
      </li>
      <li>
        <code>Beats per Bar</code> 决定游玩谱面时屏幕上显示的节拍线之间的距离。
      </li>
      <li>
        <code>Difficulty</code> 是歌曲信息上出现的难度星级。
      </li>
      <li>
        <code>Note Spacing</code> 影响游戏内note的移动速度，通常与BPM对应.
      </li>
      <li>
        <code>trackRef</code> is the globally unique name used by mods to identify your chart.
      </li>
      <li>
        <code>Song Endpoint</code> 是曲目结束时的节奏点。 这个值通常由软件自动计算，但是你可以调整这个数值来改变结算界面的出现时机。
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      点击OK。 在出现的文件选择器中，创建一个与您输入的 <code>trackRef</code> 字段相同的文件夹，并将文件命名为 <code>song.tmb</code>后放入文件夹中 。
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      您的音乐应该是一个 .ogg 文件。 您可以使用像Audacity这样的软件在音轨开始时插入一定时长的空白来将它与midi文件匹配。 将文件命名为<code>song.ogg</code>。
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      移动ogg文件到与<code>song.tmb</code>相同的文件夹。
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      按照 <a href="installing-songs">自制谱面安装说明</a> 来测试你的自制谱。
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">添加背景！</a>
    </p>
  </li>
</ol>
