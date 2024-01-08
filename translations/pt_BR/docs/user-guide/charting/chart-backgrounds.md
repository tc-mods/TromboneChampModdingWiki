# Plano de fundo para charts
---

Planos de fundo são uma característica importante de um chart, e existem alguns tipos diferentes deles (em ordem de complexidade):

### .png

Se quiser um fundo simples e fácil de se fazer, esse é o recomendado.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Se quiser um plano de fundo um pouco mais interessante, um clipe musical, ou quer pré-renderizar um fundo se movendo, você pode usar um vídeo!

Basta por um arquivo .mp4 com o nome `bg.mp4` na pasta de sua música.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Se quiser fazer um plano de fundo que vai deixar a gurizada de queixo caído, quer usar eventos, ou quer ter controle total de seu chart, recomendamos criar um arquivo `.trombackground`.

Isto lhe dará todo o poder do editor Unity, e a quantidade de coisas que você pode fazer é maior que qualquer outro método.

As instruções são atualmente encontradas num detalhado readme no GitHub do projeto Unity: <https://github.com/legoandmars/TrombLoaderBackgroundProject/> (Somente em inglês no momento.)
