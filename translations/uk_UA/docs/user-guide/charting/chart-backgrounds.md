# Фони чартів
---

Фони — важлива частина чарту, їх є пару типів (у порядку складності):

### .png

Якщо ви хочете простий, легкий фон — це найкращий вибір.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Якщо ви хочете трохи цікавіший фон, наприклад музичний кліп, або просто фон який рухається — ви також можете використовувати відео!

Просто покладіть файл формату .mp4 з назвою `bg.mp4` у папку пісні.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Якщо ви хочете фон який здивує людей, хочете використовувати події, або хочете повний креативний контроль над тим як виглядає ваш чарт — дуже рекомендовано використовувати файл `.trombackground`.

Це дасть вам повну силу Редактора Unity та більшу кількість речей які ви можете зробити в порівнянні з попередніми методами.

На даний час інструкції знаходяться в детальному readme в Unity-проєкті на GitHub: <https://github.com/legoandmars/TrombLoaderBackgroundProject/> (англ.)
