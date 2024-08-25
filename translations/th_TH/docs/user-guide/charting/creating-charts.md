# การสร้างผัง
---

?> ถ้าคุณชอบวิธีแบบวีดีโอ NyxTheShield มี [บันทึกของสตรีม](https://www.youtube.com/watch?v=ig27SlJveGs) ที่อธิบายทุกขั้นตอนในการทำผังอย่างละเอียด

## พื้นฐาน
### ตัวตัดต่อ Midi/DAW
ผังสร้างได้จากการสร้างไฟล์ MIDI และรันผ่าน [MIDI converter](#converting-midi-to-map-file)

Midi notes should be in the range 47 to 73 to match the game.<br>**NOTE:** Different editors use different values on the piano for this range.

ตัวตัดต่อ Midi ที่ฟรีและทดสอบว่าใช้ได้มี:
- [Reaper](https://www.reaper.fm/download.php)* (Range: B2-C#5)
- [LMMS](https://lmms.io/download#windows) (Range: B2-C#5)
- [FL Studio](https://www.image-line.com/fl-studio-download/)*† (Range: B3-C#6)
- [Cakewalk](https://www.bandlab.com/products/cakewalk)** (Range: B3-C#6)
- [Ableton](https://www.ableton.com/en/trial/)* (Range: B1-C#4)
- [Sekaiju](http://openmidiproject.osdn.jp/Sekaiju_en.html)
- [Trombone Charter](https://github.com/towai/TromboneCharter/releases/latest)

<sub>*ซอฟต์แวร์เต็มไม่ฟรีแต่มีใช้ทดอลงฟรีที่ทำผังได้</sub><br> <sub>**ส่งออกโน็ตไป MIDI จะได้ 2 รางโดยมาตราฐานซึ่งไม่สามารถใช้งานได้กับ Midi2TromboneChamp โดยมาตราฐาน</sub><br> <sub>†เวอร์ชั่นทดลองฟรีของ FL Studio ไม่ยอมให้คุณส่งออก MIDI แต่สามารถใช้วิธีอ้อมได้โดยบันทึกไฟล์โปรเจ็กและใช้ <a href="https://github.com/Kaydax/flp2midi/releases/latest">flp2midi</a>.</p>

<h4 spaces-before="0">
  โปรเจ็กของ Reaper
</h4>

<p spaces-before="0">
  ถ้าคุณไม่แน่ใจว่าจะใช้อะไร แนะนำให้ใช้ Reaper เพราะมันมีไฟล์โปรเจ็กดัดแปลงของ Trombone Champ มาให้:
</p>

<ul>
  <li>
    คำอธิบายพื้นฐานวิธีการใช้ตัวควบคุมของ Reaper (ในภาษาอังกฤษ)
  </li>
  <li>
    ตั้งค่าคอนฟิกที่กำหนดไว้แล้ว
  </li>
  <li>
    MIDI ตัวอย่าง
  </li>
</ul>

<p spaces-before="0">
  โปรเจ็กสามารถ<a href="https://trombone.wiki/docs/files/REAPER_Trombone_Champ_Charting_Template.zip">ดาวน์โหลดได้ที่นี่</a>
</p>

<h3 spaces-before="0">
  โน็ตปกติ
</h3>

<p spaces-before="0">
  โน็ตปกติสร้างในตัวตัดต่อ Midi และดูเหมือนกันกับในเกม เอาให้แน่ใจว่ามันมีช่องว่างระหว่างโน็ตแต่ละตัว!
</p>

<h3 spaces-before="0">
  โน็ตสไลด์
</h3>

<p spaces-before="0">
  Slides are created by connecting notes with each other. The slide will start at the beginning of the first note and end at the end of the second note.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide1.png" alt="ตัวอย่างโน็ตสไลด์" />
</p>

<p spaces-before="0">
  To create slides with multiple parts or to adjust the slide timing and curve, split up the notes in the slide.
</p>

<p spaces-before="0">
  <img src="../docs/files/slide2.png" alt="ตัวอย่างโน็ตสไลด์หลายตัว" />
</p>

<h2 spaces-before="0">
  การแปลง Midi เป็นไฟล์ผัง
</h2>

<ol start="1">
  <li>
    <p spaces-before="0">
      Go to <a href="https://tc-chart-converter.github.io/">Trombone Champ Chart Converter</a>.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      ใส่ข้อมูลในช่อง
    </p>
    <ul>
      <li>
        <code>Song Name</code> is the full name of the song, shown in the info when you select it in-game.
      </li>
      <li>
        <code>Short Name</code> แสดงชื่อในขณะที่เลือ่นผ่านรายการเพลง
      </li>
      <li>
        <code>Artist</code> is the composer of the song.
      </li>
      <li>
        <code>Release Year</code> is the year the song was created.
      </li>
      <li>
        <code>Beats per Bar</code> กำหนดความกว้างของ "เส้นโน็ต"
      </li>
      <li>
        <code>Difficulty</code> เลขดาวระดับความยากที่แสดงในข้อมูลเพลง
      </li>
      <li>
        <code>Note Spacing</code> ความเร็วที่เลเวลจะเลื่อน จะรวมกับ BPM
      </li>
      <li>
        <code>trackRef</code> is the globally unique name used by mods to identify your chart.
      </li>
      <li>
        <code>Song Endpoint</code> จังหวะที่เพลงจบ มันคำนวณอัตโนมัติแต่คุณสามารถเปลี่ยนได้ว่าเลเวลจะจบตอนไหน
      </li>
    </ul>
  </li>
  
  <li>
    <p spaces-before="0">
      กด OK Create a folder with the same name as you entered in the <code>trackRef</code> field, and save the file as <code>song.tmb</code> inside that folder.
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      แทร็กเพลงของคุณควรเป็นไฟล์ .ogg คุณสามารถใช้โปรแกรมเช่น Audacity ใส่ส่วนเงียบเข้าไปในแทร็กเพื่อที่จะให้ตรงกับ Midi ตั้งชื่อไฟล์เป็น <code>song.ogg</code>
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      ย้ายไฟล์ ogg ไปโฟล์เดอร์เดียวกันที่มี <code>song.tmb</code>
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      ทำตาม <a href="installing-songs">ขั้นตอนการลงเพลงที่กำหนดเอง</a> เพื่อทดสอบ
    </p>
  </li>
  
  <li>
    <p spaces-before="0">
      <a href="chart-backgrounds">ใส่พื้นหลัง!</a>
    </p>
  </li>
</ol>
