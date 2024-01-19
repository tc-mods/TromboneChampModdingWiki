# Chart Hintergründe
---

Hintergründe sind ein wichtiges Merkmal eines Charts, und es gibt mehrere Typen (sortiert nach Komplexität):

### .png

Wenn du einen einfachen, simplen Hintergrund willst, wird dies empfohlen.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Wenn du einen etwas interessanteren Hintergrund, wie einen Musikvideo oder einen bereits gerenderten bewegten Hintergrund möchtest, kannst du auch ein Video verwenden!

Lege einfach ein mp4 mit dem Namen `bg.mp4` in den Ordner deines Songs.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Wenn du einen Hintergrund willst, der Leute überrascht, Events verwendet oder du die volle kreative Kontrolle über das Aussehen deines Charts haben willst, ist es sehr empfehlenswert, eine `.trombackground` Datei zu verwenden.

Dies gibt dir die volle Kraft des Unity-Editors, und die Anzahl an Möglichkeiten ist deutlich höher als bei den anderen Methoden.

Die Anweisungen finden Sie derzeit in einem detaillierten Readme in dem Unity Project GitHub: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
