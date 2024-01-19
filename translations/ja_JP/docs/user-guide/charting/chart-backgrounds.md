# 譜面の背景設定
---

背景の設定は譜面作成において大事なことで、使用できるファイルの種類はいくつかあります (簡単なものから説明):

### .png

シンプルで簡単な背景が欲しいときはPNGファイル(画像)がオススメです！

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

もう少し背景をおもしろくしたいとき、ミュージックビデオを流したいときはMP4ファイル(動画)がオススメです！

使用するMP4ファイルの名前を「bg」`bg.mp4` にしたらカスタム音源のフォルダに入れてください。

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

もっとプレイするみんなを驚かせるような背景が欲しいとき、イベントを使いたいとき、譜面の見え方をより独創的にしたいときは `Trombackground` ファイルを使用することを強くオススメします！

これを使うとUnityエディターの機能をフル活用することができ、他のやり方と比べて出来ることも格段に増えます。

現在このUnityプロジェクトはGitHubに詳しい説明があるのでこちらをご覧ください: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
