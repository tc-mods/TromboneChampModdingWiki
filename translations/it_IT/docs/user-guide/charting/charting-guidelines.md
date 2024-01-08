# Charting Guidelines
---
The following guidelines are not absolute requirements. The goal is to make a chart that's fun to play. If ignoring these rules make a chart more enjoyable or engaging (e.g. Rush E), you are welcome to do so. Credits: tsunderestorm, StaticR.

## Best Practices
- Do not be off-key. If you have a poor sense of tone, ask #charting or #wip to take a look.
- Do not be off-beat. You can slow the song down in your editor to help distinguish faster rhythms.
- Do not start nor end abruptly.
  - Give at least one bar of rest before the first note, and continue your chart until the end of the song.
  - Adjust the length / song endpoint if the curtains are closing slightly before the background track ends. Do not to set the song endpoint in the tmb to be longer than the song length, or the song won't end.
- A note can be held for 4.5 seconds before running out of breath. If you have a note or slide longer than that, it's recommended to break it up so the player can catch their breath.
- Chords typically consist of 3-4 notes. The highest or lowest note usually sounds the cleanest to chart.
- Trombone Champ DOES support decimal BPMs. Trombone Charter, however, does not, so you will need to edit a decimal BPM into the .tmb another way.
- Avoid excessively long rest sections.

### Note Spacing
- Maintain note spacing appropriate for the difficulty.
  - As a very general guideline, the note and space between it and the next note should be of equal length
  - **IDEAL**:
  - ![Ideal Note Spacing](../docs/files/charting/ideal-note-spacing.png)
  - **NOT IDEAL**: (this might sound good in preview or autotoot but does not provide much time for a player to release and hit the next note)
  - ![Bad Note Spacing](../docs/files/charting/bad-note-spacing.png)
  - You may make exceptions:
    - to emphasize [articulation](https://people.carleton.edu/~jellinge/m101s12/Pages/04/04Articulation.html) like slurs, staccato, or legato
    - to make it easier to maintain combo on very fast sections
    - if the song tempo is very slow and a tight spacing is adequate
- The rhythm should be visually intuitive. If notes are slightly longer, they should be slightly longer visually. If notes are slightly shorter, they should be slightly shorter visually.
  - **IDEAL**: (easy to see which are eighth notes and which are dotted eighth (3/16) notes)
  - ![Ideal Visual Rhythm](../docs/files/charting/ideal-visual-rhythm.png)
  - **NOT IDEAL**: (all notes read as eighth notes)
  - ![Bad Visual Rhythm](../docs/files/charting/bad-visual-rhythm.png)
- Use a reasonable `savednotespacing` (scroll speed) value
  - 120~200, depending on song complexity. A good guideline is `100/[BPM]*280`.
  - This should be fast enough for the rhythm to be visually intuitive and slow enough that the player has time to react.
  - This value does not have to be the same as the tempo!

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
- When charting runs, simplify slides for a consistent stream of notes going up or down.
  - Instead, you can just do one single slide and pull back the end point until the slide curve matches the notes.
  - Making each individual note part of the slide will make the slide very wobbly. You can make an exception if you specifically want the slide to look like this or the note shape is too complex to estimate with one slide.
- Vibrato or trill type slides work great if they connect in the middle of the note.
- Generally, slides are cleaner with fewer connecting points.
- In a very slide heavy track, setting the color to a solid color instead of a 2 color gradient could look way cleaner.
- If you want clean slides with a midi converter, use [TCCC](https://rshieldsprojects.github.io/projects/tccc/)'s custom slide method.
- Slides can only go 1 octave both up and down from the starting note. If you want a chart a slide that spans a greater range, you can break it up in between and/or find a place where you can start the slide towards the middle of the screen.
- You can connect multiple notes at the same pitch as a slide. This plays as one continuous held note. This boosts combo count and champ meter extremely quickly, which may be useful for certain effects and gimmicks, but you wouldn't want to use it outside of that.
- Good slide timings seem to be about 2:1 to 5:1  (slide end late by about half to one 5th of the length of the slide)
  - 1:1 works too for things like trills or vibrato.
  - When in doubt, just putting the slide end a 32nd note late tends to work well for most slides.
- 2 16th notes or shorter connected work completely fine with only one slide, there doesn't need to be any held for it to sound ok, unless it is a very large jump.
- Slide ends don't need a held part, they're fine just ending a bit early (if the slide end is already delayed by the appropriate amount)

### Tap Notes
- Tap notes or dot notes are notes that show up as a single dot on screen.
- You can create tap notes by setting the note duration to be 0.06 or below.
  - The exact value you choose affects how many points the note will give and how wide of a time window the user has to hit the note. For this reason, it is recommended to always set tap note values to 0.06 for maximum ease of playability.
- Note that for most users, tap notes tend to be very difficult to accurately hit. Ideally, tap notes should only be used in places where the spacing does not allow for short held notes to be used instead.

### Looping Tracks
- A few repetitions are fine, but avoid repeating the same note pattern over and over.
  - You can look for a TV version or edit it yourself if you want a shorter version of the song.
  - Generally, it flows best if you chart the easier or more expected parts in the first play, and switch to alternatives:
    - Often, there's a primary and secondary melody.
    - Follow the chords or bassline.
    - Play it in a different octave.
    - If you know what you're doing musically, use different chords or harmonies.
  - You may want to reverse this if the main part serves as a high point in the music. Musical high points typically fit best at around the last third or quarter of the entire track, so structuring a loop like that can make it feel more complete.
- Really short tracks are best looped until about 1 to 1:30 minutes, unless they are really repetitive.
- You may choose to add a full or partial loop if there are different parts to play in a section.
- Ending a track that endlessly loops can be hard. Suggestions:
  - End at the end without any loop back.
  - End at the first beat, chord, or section of the loop.
  - Fade the music out at the end of a musical phrase.

## Technical Requirements
- Don't just convert the .mp3 to .mid. This converts all the instruments, but we can only play one note at a time. Finding a MIDI online would also likely not work without a lot of editing.
- Have [beat](https://en.wikipedia.org/wiki/Beat_(music)#On-beat_and_off-beat) markers that line up with the background audio (unless the song has a varying tempo).
- Use an audio editing software like [Audacity](https://www.audacityteam.org/) to add/remove silence to the beginning of a song to help line up the audio file’s beats with the chart’s beats.
- Ensure that the chart is perfectly synced with the background audio.
- Use [AutoToot](https://github.com/TomDotBat/AutoToot) or [Boner Viewer](https://paturages.github.io/boner-viewer/) and listen if the notes are consistently early or late.
- Set a difficulty rating consistent with [TootTally](https://toottally.com/upload/).
- Have a relevant background. A static PNG background is OK.
- Have good visual contrast between the notes and the background.
- If necessary, reduce the loudness of the song (via Audacity, etc.) so that the trombone sound can be clearly heard over the background track.
  - -15dB LUFS is a good starting point and the default export setting in the reaper template.

### File Specifications
- Follow this archive format: `[mychart].zip/[mychart]/[files]`
- Double check for invalid metadata in the .tmb file
  - `trackref` should be unique and not something like `"trackref"="trombone_charter_x64"`.
  - Check that the [json is valid](https://jsonformatter.curiousconcept.com/#).
