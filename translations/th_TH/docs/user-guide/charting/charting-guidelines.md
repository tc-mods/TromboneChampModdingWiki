# ข้อแนะนำการทำเพลง
---
ข้อแนะนำพวกนี้ไม่จำเป็นที่จะต้องทำตามก็ได้ จุดประสงค์ก็คือเพลงนั้นสนุกที่จะเล่น ถ้าเลือกที่จะไม่สนใจกฎก็ทำเพลงให้เล่นให้หรือน่าสนใจ (เช่น Rush E) ก็ยินดีที่จะให้ทำ เครดิต: tsunderestorm, StaticR.

## แบบอย่างที่ดี

- รักษาระยะห่างของโน็ตให้เหมาะสมกับความยาก
  - นี่เป็นข้อแนะนำทั่วไป โน็ตและระยะห่างระหว่างโน็ตตัวต่อไปควรที่จะมีความยาวเท่ากัน
  - **ควร**:
  - ![Ideal Note Spacing](../docs/files/charting/ideal-note-spacing.png)
  - **ไม่ควร**: (นี่อาจจะให้เสียงดีสำหรับการดูตัวอย่างหรือใช้ autotoot แต่มันไม่ให้เวลาพอที่จะปล่อยและกฎโน็ตต่อไปสำหรับคนเล่น)
  - ![Bad Note Spacing](../docs/files/charting/bad-note-spacing.png)
  - คุณสามารถใช้ข้อยกเว้นได้เมื่อ:
    - เพื่อเน้น[การประกบ](https://people.carleton.edu/~jellinge/m101s12/Pages/04/04Articulation.html) เช่น การทอดเสียง การขาดตอน หรือ การเล่นค่อยๆโดยไม่ขาดเสียง
    - เพื่อทำให้การทำคอมโบง่ายขึ้นในส่วนเร็ว
    - ถ้าเกิดจังหวะเพลงนั้นช้าและช่องว่างที่แน่นเพียงพอ
- อย่าทำให้โน็ตเพี้ยน ถ้าคุณได้ยินระดับเสียงไม่ดี ถาม #charting หรือ #wip ให้มาช่วยดู
- อย่าทำให้ผิดจังหวะ คุณสามารถชะลอเพลงในตัวตัดต่อของคุณเพื่อช่วยแยกแยะจังหวะที่เร็วของเพลง
- อย่าเริ่มหรือหยุดเพลงกะทันหัน
  - ให้อย่างน้อยช่องว่างช่องหนึ่งก่อนโน็ตตัวแรกและทำเพลงต่อไปไปจนจบเพลง
  - ปรับ ความยาว/จุดจบของเพลง ถ้าผ้าม่านกำลังปิดก่อนที่เพลงจะหยุด อย่าตั้งจุดจบของเพลงใน tmb ยาวกว่าความยาวของเพลงไม่อย่างนั้นเพลงจะไม่หยุด
- จังหวะเพลงควรที่จะมองเห็นได้ง่าย ถ้าโน็ตยาวกว่านิดหน่อยมันก็ควรที่จะเห็นยาวกว่านิดหน่อย ถ้าโน็ตสั้นกว่านิดหน่อยมันก็ควรที่จะเห็นสั้นกว่านิดหน่อย
  - **ควร**: (เห็นได้ง่ายว่าตัวไหนเป็นโน็ตตัวสั่นและตัวไหนเป็นโน้ตประจุด (3/16))
  - ![Ideal Visual Rhythm](../docs/files/charting/ideal-visual-rhythm.png)
  - **ไม่ควร**: (โน็ตทุกตัวเป็นโน็ตตัวสั่น)
  - ![Bad Visual Rhythm](../docs/files/charting/bad-visual-rhythm.png)
- ใช้ค่า `savednotespacing` (ความเร็วของการเลื่อน) ให้เหมาะสม
  - 120~200 ขึ้นอยู่กับความซับซ้อนของเพลง แนวทางที่ดีคือ `100/[BPM]*280`
  - นี่ควรเร็วพอที่ทำให้จังหวะเห็นได้ง่ายและช้าพอที่ให้ผู้เล่นมีเวลาที่จะตอบสนอง
  - ค่านี้ไม่จำเป็นที่จะต้องเหมือนกับจังหวะ!
- โน็ตสามารถยาวได้ถึง 4.5 วินาทีกอนที่จะหมดลมหายใจ ถ้าคุณมีโน็ตหรือสไลด์ที่ยาวกว่านั้น แนะนำว่าให้แยกมันเพื่อให้ผู้เล่นมีเวลาหายใจ
- คอร์ดโดยทั่วไปประกอบด้วยโน็ต 3-4 ตัว โน็ตสูงสุดหรือต่ำสุดโดยปกติให้เสียงที่สะอาดที่สุดสำหรับเพลง

### แทร็กวนซ้ำ
- วนซ้ำนิดหน่อยไม่เป็นไรแต่หลีกเลี่ยงวนซ้ำโน็ตไปเรื่อยๆ
  - คุณสามารถหาเวอร์ชั่นทีวีหรือตัดต่อด้วยตัวเองถ้าคุณยากได้เพลงที่สั้นลง
  - โดยทั่วไป มันไปได้ดีถ้าคุณทำเพลงที่ง่ายหรือส่วนที่คาดไว้มากในการเล่นครั้งแรก และเลี่ยนไปเป็นอย่างอื่น
    - มันมีทำนองหลักและทำนองรองบ่อยครั้ง
    - ไปตามกับคอร์ดหรือเบสไลน์
    - เล่นอ็อกเทฟที่ต่างกัน
    - ถ้าคุณรู้ว่ากำลังกำลังทำอะไรในทางดนตรี ใช้คอร์ดหรือฮาร์โมนีอย่างอื่น
  - คุณอาจอยากที่จะห้วนกลับถ้าส่วนหลักเป็นจุดสูงสุดของเพลง Musical high points typically fit best at around the last third or quarter of the entire track, so structuring a loop like that can make it feel more complete.
- Really short tracks are best looped until about 1 to 1:30 minutes, unless they are really repetitive.
- You may choose to add a full or partial loop if there are different parts to play in a section.
- Ending a track that endlessly loops can be hard. Suggestions:
  - End at the end without any loop back.
  - End at the first beat, chord, or section of the loop.
  - Fade the music out at the end of a musical phrase.

### Slides
- Avoid 90 degree slide angles.
  - **IDEAL**: (player has adequate time to change pitches. Depending on latency, you might want to adjust the position of the connecting points.)
  - ![Ideal Slide 1](../docs/files/charting/ideal-slide1.png)
  - **MAYBE IDEAL**: (only if a quick transition is absolutely necessary)
  - ![Ideal Slide 2](../docs/files/charting/ideal-slide2.png)
  - **NOT IDEAL**: (this is not humanly playable)
  - ![Bad Slide](../docs/files/charting/bad-slide.png)
- A slide approaches the target pitch before the slide end.
  - Make the end of the slide ~1-2 32nd notes late, depending on the length of the slide.
  - Start the slide about one 16th note before the target beat. It'll still be fine if half the note is a slide.
- For 8th note slides or shorter, you don't need to include a held note in the middle.
  - You often don't need a held note at the slide start, middle or end at all, unless you want the note to be clearly held for an 8th note or longer.
- Simplify slides for a consistent stream of notes going up or down.
  - Instead, you can just do one single slide and pull back the end point until the slide curve matches the notes.
  - Making each individual note part of the slide will make the slide very wobbly. You can make an exception if you specifically want the slide to look like this or the note shape is too complex to estimate with one slide.
- Vibrato or trill type slides work great if they connect in the middle of the note.
- Generally, slides are cleaner with fewer connecting points.
- In a very slide heavy track, setting the color to a solid color instead of a 2 color gradient could look way cleaner.
- If you want clean slides with a midi converter, use [TCCC](https://rshieldsprojects.github.io/projects/tccc/)'s custom slide method.
- Slides can only go 1 octave both up and down from the starting note. If you want a chart a slide that spans a greater range, you can break it up in between and/or find a place where you can start the slide towards the middle of the screen
- You can connect multiple notes at the same pitch as a slide. This plays as one continuous held note. This boosts combo count and champ meter extremely quickly, which may be useful for certain effects and gimmicks, but you wouldn't want to use it outside of that.
- Good slide timings seem to be about 2:1 to 5:1  (slide end late by about half to one 5th of the length of the slide)
  - 1:1 works too for things like trills or vibrato.
  - When in doubt, just putting the slide end a 32nd note late tends to work well for most slides.
- 2 16th notes or shorter connected work completely fine with only one slide, there doesn't need to be any held for it to sound ok, unless it is a very large jump.
- Slide ends don't need a held part, they're fine just ending a bit early (if the slide end is already delayed by the appropriate amount)

## Technical Requirements
- Don't just convert the .mp3 to .mid. This converts all the instruments, but we can only play one note at a time. Finding a MIDI online would also likely not work without a lot of editing.
- Have [beat](https://en.wikipedia.org/wiki/Beat_(music)#On-beat_and_off-beat) markers that line up with the background audio (unless the song has a varying tempo).
- Use an audio editing software like [Audacity](https://www.audacityteam.org/) to add/remove silence to the beginning of a song to help line up the audio file’s beats with the chart’s beats.
- Ensure that the chart is perfectly synced with the background audio.
- Use [AutoToot](https://github.com/TomDotBat/AutoToot) or [Boner Viewer](https://paturages.github.io/boner-viewer/) and listen if the notes are consistently early or late.
- Set a difficulty rating consistent with [TootTally](https://toottally.com/upload/).
- Avoid excessively long rest sections.
- Have a relevant background. A static PNG background is OK.
- Have good visual contrast between the notes and the background.
- If necessary, reduce the loudness of the song (via Audacity, etc.) so that the trombone sound can be clearly heard over the background track.
  - -15dB LUFS is a good starting point and the default export setting in the reaper template.

### File Specifications
- Follow this archive format: `[mychart].zip/[mychart]/[files]`
- Double check for invalid metadata in the .tmb file
  - `trackref` should be unique and not something like `"trackref"="trombone_charter_x64"`.
  - Check that the [json is valid](https://jsonformatter.curiousconcept.com/#).
- Use h.264 as the video codec for maximum compatibility.
- Have an appropriate video file size (target 10MB per minute of song)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.
