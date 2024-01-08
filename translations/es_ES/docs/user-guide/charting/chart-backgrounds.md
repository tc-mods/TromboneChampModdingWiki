# Fondo de Mapa
---

Los fondos son una característica importante de un mapa, y hay unos diferentes tipos (en orden de complejidad):

### .png

Si quieres un fondo simple y fácil, esto se recomienda.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

¡Si quieres un fondo un poco más interesante, un fondo de video musical, o pre renderizar un fondo en movimiento, puedes usar un video!

Simplemente pon un mp4 llamado `bg.mp4` en la carpeta de tu canción.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Si quieres un fondo que hará volar a la gente, quieres usar eventos, o quieres total control creativo de cómo se ve tu mapa, es altamente recomendado usar un archivo `.trombackground`.

Esto te dará el poder total del editor de Unity, y la cantidad de cosas que puedes hacer es significativamente mayor que con cualquiera de los otros métodos.

Las instrucciones se encuentran en un detallado readme en el Unity Project Github: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
