# 채보 배경
---

배경은 채보 제작의 중요한 기능이며, 사용할 수 있는 파일 종류에는 몇 가지 유형이 있습니다 (간단한 것부터 설명):

### .png

심플하고 간단한 배경을 원할 때는 이미지 파일을 추천합니다.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

조금 더 재미있는 배경을 만들고 싶을 때나, 뮤직 비디오를 재생하고 싶을 때에는 동영상 파일을 추천합니다.

`bg.mp4`라는 이름의 동영상 파일을 음악 폴더에 넣기만 하면 됩니다.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

플레이하는 모두를 놀라게 할 만한 배경을 원할 때, 이벤트를 사용하고 싶을 때, 채보를 보다 독창적으로 만들고 싶을 때는 `.trombackground` 파일을 사용하는 것을 강력히 추천합니다.

이를 사용하면 Unity 에디터의 모든 기능을 사용할 수 있고, 다른 방법에 비해 더욱 많은 작업을 할 수 있습니다.

현재 이 Unity 프로젝트는 GitHub에 자세한 설명이 있으므로 여기를 참고해주세요: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
