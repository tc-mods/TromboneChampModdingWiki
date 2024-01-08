# 谱面制作指导
---
以下内容仅为指导意见，并非绝对的硬性要求。 一切指导意见的最终目的都是制作一个游玩体验足够优秀的自制谱面。 如果忽略这些意见能够使你的谱面更有趣或者更具有吸引力（例如 Rush E），那么按照您自己的方式去制作即可。 编写者: tsunderestorm, StaticR. （译者：Bilibili@银狐V933 Discord@SilverFoxV933，以下内容较为抽象，看不懂不要太在意，实在想了解可以来b站直接与我交流。译者从未系统学过乐理相关知识。对于部分用词不准确或混乱的情况，还望海涵。）

## 游玩体验最佳化
- 请勿跑调。 如果您音感不佳，可以向#charting或#wip请求协助。
- 请注意节奏。 您可以在编辑谱面时适当减慢乐曲的速度以应对较快的节奏。
- 开始与结束应尽可能自然。
  - 在第一个note之前留出至少一个小节的空白距离，并保证你的谱面能持续到乐曲结束。
  - 在谱面的.tmb文件中调整谱面的结束点（endpoint）以确保结算画面不会过早出现。 结束点推荐设置在乐曲最后一个音结束到乐曲文件结束之间。不要设置在乐曲文件结束之后，会导致无法结算。
- 一个长note的极限长度为4.5秒，超过这个时间会触发强制的换气惩罚。 推荐对超过这个时间的长note进行拆分以便玩家有时间换气。
- 和弦通常包含3到4个note。 选择最高或最低的note写入谱面，效果最好。
- Trombone Champ DOES support decimal BPMs. Trombone Charter, however, does not, so you will need to edit a decimal BPM into the .tmb another way.
- 避免出现过长的休息段。

### Note Spacing
- 保证note间距与难度相匹配
  - 通常情况下，note与note之间的间隔应该与note本身同长。
  - **正面示例**:
  - ![理想的note间距](../docs/files/charting/ideal-note-spacing.png)
  - **反面示例**: （这种排布虽然在自动演奏中可能会拥有较好的听感，但没有足够的时间空档让玩家抬手并点击下一个note。）
  - ![糟糕的note间距](../docs/files/charting/bad-note-spacing.png)
  - 当遇到以下情形时，可不遵守此项：
    - 突出表达音调的[连续性](https://people.carleton.edu/~jellinge/m101s12/Pages/04/04Articulation.html)。比如连奏，断奏和延长音
    - 在较快速的段落简化谱面以保持Combo。
    - 曲目的节奏较慢，以至于可以使用较紧凑的note排布。
- 谱面节奏应足够直观。 如果一个note略微更长，这种长度区别在实际游玩时应该能被明显地辨认出。 短note同理。
  - **正面示例**: （可以直观的分辨note的长短）
  - ![理想的节奏视觉表现](../docs/files/charting/ideal-visual-rhythm.png)
  - **反面示例**: （所有note看起来长度相等）
  - ![糟糕的节奏视觉表现](../docs/files/charting/bad-visual-rhythm.png)
- 选择一个合适的 `savednotespacing` （滚动速度）。
  - 通常在120~200的区间内，取决于谱面的复杂程度。 推荐使用 `100/[BPM]*280`.
  - 理想的谱面流速，应该是能让谱面的节奏得以直观展现的同时，足以让玩家有时间对谱面作出反应。
  - 这个值不必与BPM相同！

### 滑动（slide）note
- 避免出现接近90度的滑动操作。
  - **正面示例**: （玩家有足够的时间改变音高。 考虑到延迟，您可能需要调整滑动note连接点的位置。）
  - ![理想的滑动note 1](../docs/files/charting/ideal-slide1.png)
  - **可接受的示例**: （仅在有必要使用快速过渡时。）
  - ![理想的滑动note 2](../docs/files/charting/ideal-slide2.png)
  - **反面示例**: （不是人玩的东西-_-）
  - ![糟糕的滑动note](../docs/files/charting/bad-slide.png)
- 滑动note的滑动部分到达目标音高的时间比滑动部分结束要提前一点。
  - 将滑动部分的结束点延后1~2/32音符的长度。
  - 滑动部分的起始点提前1/16音符。 适合滑动note中滑动部分占比超过一半的情况。
- 对于等于或短于1/8音符的滑动note，不建议滑动部分中间分段。
  - 一个滑动note可以不在开始，中途或结束保留任何非滑动部分。
- When charting runs, simplify slides for a consistent stream of notes going up or down.
  - 同方向的多段滑动可以合并为单个滑动，通过调整滑动部分结束点来与实际的音调匹配。
  - 一段滑动中每一个note都保留会使得滑动部分过于波动。 尽量避免这种情况，除非您有意为之或原曲音调过于复杂无法用单个滑动来表现。
- 抖动音或颤音建议从每个音的中间进行连接。
- 通常情况下，分段越少的滑动效果越好。
- 如果谱面中滑动轨道较多，建议设置note颜色时头尾选择相同的颜色，可增强谱面观感。
- 除了旧有的滑动note编写方式，还可以尝试 [TCCC](https://rshieldsprojects.github.io/projects/tccc/)转换器采用的新的编写方式，对于编写滑动note有一定的帮助。
- 滑动note滑动的最大范围为一个八度。 If you want a chart a slide that spans a greater range, you can break it up in between and/or find a place where you can start the slide towards the middle of the screen.
- 您无法将同音高的note连接成滑动note。 这种情况下游玩起来与普通长note相同。 与普通长note不同的是它可以以极快的速度累积Combo数，在某些特殊场合可能会比较有用，但也仅此而已，不应滥用。
- 适宜的滑动note时间比例通常为2:1到5:1（滑动部分的结束点延后一般到五分之一的整个滑动note长度）。
  - 1:1 通常适用于抖动音或颤音。
  - 如有疑惑，只要将滑动部分的末尾延后1/32音符就能适配绝大多数滑动note的情况。
- 1/8或更短音符仅需单个滑动部分即可，不需要额外在中间放置note分段就可以有不错的听感，除非是大范围的跳跃。
- 滑动note的结尾不必保留停顿的部分，在滑动部分的结束点已经按照前文所说提前了的情况下已经不在需要额外保留停顿。（译者注：以上内容看不懂也没关系，多写写就懂了。其实我很多也不懂……）

### Tap Notes
- Tap notes or dot notes are notes that show up as a single dot on screen.
- You can create tap notes by setting the note duration to be 0.06 or below.
  - The exact value you choose affects how many points the note will give and how wide of a time window the user has to hit the note. For this reason, it is recommended to always set tap note values to 0.06 for maximum ease of playability.
- Note that for most users, tap notes tend to be very difficult to accurately hit. Ideally, tap notes should only be used in places where the spacing does not allow for short held notes to be used instead.

### 乐曲结构
- 允许存在一定的重复。但要避免同一个note排布过度反复地出现。
  - 选曲时，可以考虑选择TV版（如果有的话），或亲手编辑以获得较短版本的乐曲。
  - 通常情况下，在两个重复的段落中，首段采用较为简单或较为明显的部分来作谱，复段则采用其他部分，这类分配效果最好。
    - 一个乐曲段落通常由主副两段旋律（或多段）合成。
    - 尝试采用和弦或低音声部。
    - 高（或低）一个八度来演奏。
    - 如果您对您的乐感比较有自信，可以尝试自己编写合适的和声。
  - 应尽可能避免乐曲的高潮桥段出现的过早。 音乐高点通常最适合出现在整个曲目的最后三分之一或四分之一左右，照此调整整个乐曲的结构可以让乐曲显得更加完整。
- 较短的乐曲应该循环至1:00到1:30之间，除非重复性过高。
- 如果您对某个段落打算编写多个不同的排布，您可以选择对其添加一个完整或部分的循环。
- 对于一个无限循环的乐曲来说，可能会较难寻找结束点。 建议您：
  - 在单次循环结束时直接结束，不做任何循环。
  - 在循环的第一个节奏点，第一个和弦或第一个小节结束循环。
  - 在乐曲末尾添加淡出效果。

## 技术性要求
- 请勿直接将.mp3转换为.mid（译者注：即自动扒谱）。 这类转换通常无法提取出单独的某一种乐曲或声部，而我们在游戏中一次只能弹奏一个note。 即便寻找现成的midi文件，在放入转换器转换为可玩的谱面之前通常也免不了大量的编辑。
- 在转换谱面时记得设定小节线（[beat](https://en.wikipedia.org/wiki/Beat_(music)#On-beat_and_off-beat) markers）并与音乐对齐，除非乐曲的bpm有变化。
- 使用音频编辑软件（例如[Audacity](https://www.audacityteam.org/)）调整乐曲开头的空白部分的时长来让乐曲的节奏与谱面的节奏对齐。
- 保证谱面与乐曲的同步性。
- 使用 [AutoToot](https://github.com/TomDotBat/AutoToot) 或[Boner Viewer](https://paturages.github.io/boner-viewer/) 检验谱面中的note是否有持续性的提前或延后现象。
- 使用[TootTally](https://toottally.com/upload/)来给你的谱面进行难度定级。
- 记得添加一个合适的背景。 一个静态PNG图片就足够了。
- 谱面上的note在背景上应有足够的辨识度，可以考虑调整note颜色或将背景略微调暗。
- 如有必要，减小乐曲的音量（使用Audacity或其他）以保证长号的声音能被清晰地听到。
  - -15dB LUFS 效果比较不错，是Reaper自制文件示例中的默认导出设置。（译者注：实际要根据不同曲目的音量情况进行单独调整，推荐实际去游戏中进行实地测试。此外乐曲音量应该减弱多少还与当前曲目是否有声部容易与长号的声音发生混合有关。举例来说如果你的音乐是去掉了人声的流行乐，而在写谱时选择用长号代替人声，则乐曲音量就不需要降得太低。无论如何最终仍应以游戏内实际测试为准。）

### 文件规格
- 推荐使用的压缩包命名以及压缩包内容的格式：`[mychart].zip/[mychart]/[files]`
- 反复检查.tmb文件中涉及的谱面基本数据。
  - `trackref` 应该是唯一的，而不是类似 `"trackref"="trombone_charter_x64"`.
  - 确认谱面文件.tmb中的 [json代码](https://jsonformatter.curiousconcept.com/#)准确无误。（译者注：链接是一个json语句纠错的网站，用记事本打开.tmb文件并复制全部文本至这个网页，点Process就可以检测文件是否有语法上的错误，防止出现一些意想不到的情况。）
