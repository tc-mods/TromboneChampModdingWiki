# Arrière-plans des chansons personnalisées
---

Les arrières-plans sont une fonctionnalité importante des charts, et il y en a quelques types différents (en ordre de complexité):

### .png

Si vous voulez un arrière-plan simple et facile, c'est ce qui est recommandé.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Si vous voulez un arrière-plan un peu plus intéressant, un fond vidéo de musique, ou si vous préférer un arrière-plan en mouvement, vous pouvez également utiliser une vidéo !

Mettez simplement un mp4 nommé `bg.mp4` dans le dossier de votre chanson.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Si vous voulez un arrière-plan qui va époustoufler les gens, utiliser des événements, ou souhaitez avoir un contrôle créatif complet de l'apparence de votre chanson personnalisée, il est fortement recommandé d'utiliser un fichier ` .trombackground`.

Cela vous donnera toute la puissance de l'éditeur Unity, et la quantité de choses que vous pouvez faire est beaucoup plus élevée que l'une des autres méthodes.

Les instructions se trouvent actuellement dans un lisezmoi détaillé sur GitHub du projet Unity : <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
