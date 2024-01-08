# Sfondi della Chart
---

Gli sfondi sono una caratteristica importante di una chart e ne esistono diversi tipi (in ordine di complessità):

### .png

Consigliato per chi vuole uno sfondo semplice e facile da realizzare.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Per chi vuole uno sfondo un po' più interessante, un video musicale in sottofondo, o pre-renderizzare uno sfondo in movimento. Si può usare anche un video!

Basta mettere un file mp4 rinominato `bg.mp4` nella cartella della canzone.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Se vuoi uno sfondo che lascerà la gente a bocca aperta, se vuoi usare degli eventi, o se vuoi avere il pieno controllo creativo sull'aspetto della tua chart, è altamente raccomandato usare un file `.trombackground`.

In questo modo avrai il pieno potere del'Editor di Unity, e la quantità di cose che potrai fare è decisamente maggiore rispetto ai metodi precedentemente descritti.

Le istruzioni possono essere trovate in un file "readme" nel GitHub del progetto Unity: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
