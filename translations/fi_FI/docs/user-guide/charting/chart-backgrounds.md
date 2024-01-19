# Kartan Taustat
---

Taustat ovat tärkeä osa karttaa, ja niitä on muutamia eri tyyppejä (monimutkaisuus järjestyksessä):

### .png

Jos haluat yksinkertaisen, helpon taustan, tämä on mitä suositellaan.

Simply put a `1780x1000` image named `bg.png` in your song's folder.

You can use non-`1780x1000` images, but it might behave weirdly, as unity sprite scale is based on image resolution. If your image is too small it will have an ugly grey background to fill the remaining space.

### .mp4

Jos haluat hieman mielenkiintoisemman taustan, musiikkivideon taustan tai haluat ennakoida liikkuvaa taustaa, voit käyttää myös videota!

Laita vain 1920x1080 video nimellä `bg.mp4` kappaleesi kansioon.

- Use h.264 as the video codec for maximum compatibility.
- You can use any resolution of video, but **please** try to keep the size reasonable. (target 10MB per minute of song - aim for under 50MB)
  - Use a tool like [Handbrake](https://handbrake.fr/) to reencode and compress video.
  - Use two-pass encoding with a target bitrate of 1333kbps to eliminate any guesswork.
  - Remove the audio track entirely.

### .trombackground

Jos haluat taustan, joka hämmästyttää ihmisiä, haluat käyttää tapahtumia, tai haluat olla täysin luova ohjaus miten kartta näyttää, on erittäin suositeltavaa käyttää `.trombackground` tiedostoa.

Tämä antaa sinulle täyden voiman Unity Editoriin, ja määrä asioita joita voit tehdä on huomattavasti suurempi kuin kumpikaan muista menetelmistä.

Ohjeet löytyvät Unity Project GitHubista yksityiskohtaisesta lukemasta: <https://github.com/legoandmars/TrombLoaderBackgroundProject/>
