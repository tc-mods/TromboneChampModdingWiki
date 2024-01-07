# Chart Backgrounds
---

Backgrounds are an important feature of a chart, and there's a few different types (in order of complexity):

### .png

If you want a simple, easy background, this is what's recommended. 

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1920x1080` images, but it might behave weirdly, as unity sprite scale is based on image resolution.

### .mp4 

If you want a slightly more interesting background, a music video background, or want to prerender a moving background, you can also use a video!

Simply put an mp4 named `bg.mp4` in your song's folder.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

If you want a background that'll blow people away, want to use events, or want to have full creative control of how your chart looks, it's highly recommended to use a `.trombackground` file.

This will give you the full power of the Unity Editor, and the amount of things you can do is significantly higher than either of the other methods.

The instructions are currently found in a detailed readme on the Unity Project GitHub: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
