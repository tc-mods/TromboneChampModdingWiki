# พื้นหลังของเพลง
---

พื้นหลังเป็นฟีเจอร์ที่สำคัญของผังและมีความแตกต่างบางประการ (ตามลำดับความซับซ้อน)

### .png

อันนี้แนะนำถ้าคุณอยากได้พื้นหลังแบบง่ายๆ

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

ถ้าคุณอยากได้พื้หลังที่น่าสนใจมากขึ้น, มิวสิควิดีโอ หรืออยากให้พื้นหลังเคลื่อนไหว คุณสามารถใช้วีดีโอได้!

แค่ใส่วีดีโอ mp4 และเปลี่ยนชื่อเป็น `bg.mp4` ในโฟลเดอร์เพลงของคุณ

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

ถ้าคุณอยากได้พื้นหลังที่จะทำให้คนตะลึง, อยากจะใช้อีเวนท์, หรืออยากจะสร้างสรรค์เต็มความสามารถของผังของคุณ แนะนำอย่างสูงให้ใช้ไฟล์ `.trombackground`

นี่จะทำให้คุณมีอำนาจจาก Unity Editor เต็มที่และหลายอย่างที่สามราถทำได้สูงกว่าจากวิธีที่กล่าวมา

ขั้นตอนอยู่ใน readme บน Unity Project GitHub <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
