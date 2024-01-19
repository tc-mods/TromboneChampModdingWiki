# 自制谱面背景
---

背景是一个谱面的重要组成部分，下面介绍背景的几种不同的类型（以复杂程度从简至繁排序）：

### .png

如果您想要一个简单直接的背景，推荐使用这个格式。

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

如果您想要稍微更有趣的背景，例如一个音乐视频，或者单纯想要一个预渲染的动态的背景，您也可以使用视频文件！

只需在您的歌曲文件夹中放入名称为`bg.mp4`的视频。

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

如果您想要一个能令人瞠目结舌的背景，想要使用事件，或想要完全地创造性地控制您的自制谱面外观，强烈建议您使用 `.trombackground` 文件。

这个格式允许您使用Unity Editor的全部功能。您的编辑自由度会远远高于其他任何一种背景形式。

目前在Unity Project GitHub有一个详细的指南：<https://github.com/legoandmars/TrombLoaderBackgroundProject/>
