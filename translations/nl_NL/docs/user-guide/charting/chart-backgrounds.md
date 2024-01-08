# Map Achtergrond
---

Achtergronden zijn een belangrijke functie van een map, en er zijn een paar verschillende types (in volgorde van complexiteit):

### .png

Als je een eenvoudige achtergrond wilt, wordt dit aanbevolen.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Als je een iets interessantere achtergrond wilt, zoals een muziekvideo of een bewegende achtergrond, kun je ook een video gebruiken!

Plaats dan een mp4 genaamd `bg.mp4` in de songmap.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Als je een achtergrond wil die mensen wegblaast, als je events wil gebruiken of gewoon volledige creatieve controle hebben over hoe je map eruit ziet, wordt het sterk aanbevolen om een `.trombackground` bestand te gebruiken.

Dit geeft je de volledige kracht van de Unity Editor, en de hoeveelheid dingen die je kunt doen is een stuk groter dan met de andere methoden.

De instructies zijn momenteel gevonden in een gedetailleerde readme op Unity Project GitHub: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
