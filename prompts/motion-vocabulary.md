# 动效与创意词汇提示词

每条提示词原文照录在代码块里，不改写、不翻译；中文含义和用法写在下面。编号与 `image-generation.md` / `video-generation.md` 共用一套（全库连续编号）。

本分类收录的是「专业效果名称 + 向 AI 怎么说」的例句合集，完整效果库在开源仓库 [showheyohtaki/motion-prompt](https://github.com/showheyohtaki/motion-prompt)（192 条），这里只摘代表性条目，避免整库照搬。

| 编号 | 标题 | 用途 | 场景 | 适用工具 | 来源 |
| --- | --- | --- | --- | --- | --- |
| p006 | [Motion Prompt 精选例句（192 条效果库摘录）](#p006-motion-prompt-精选例句192-条效果库摘录) | 用专业名称 + 参数向 AI 描述动效 / 镜头 / UI / 摄影效果 | 落地页动效、视频运镜、UI 动画、布光提示词 | Claude Code / Codex（可装 motion-prompt Skill） | [@ChatGptAstra 2026-11-09](https://x.com/ChatGptAstra/status/2119732495747043631) |

## p006 Motion Prompt 精选例句（192 条效果库摘录）

```text
#001 弹性入场（Pop-in）：元素弹跳着出现
向 AI：让标志以弹性入场出现，时长约 0.4 s，略微超出目标尺寸后回弹。

#002 交错动画（Stagger）：多个元素错开时间依次出现
向 AI：用交错动画让五张卡片从左到右依次入场，每张间隔 0.08 s。

#025 水平摇镜头（Pan）：机位固定，向左或右转动镜头
向 AI：固定机位，用 5 s 从左向右缓慢摇摄城市天际线。

#032 滑动变焦（Dolly zoom (Vertigo)）：主体大小不变，背景发生透视变化
向 AI：在人物顿悟时做滑动变焦：保持脸的大小，让背景拉远。

#049 模态对话框（Modal dialog）：打开浮窗并暂时阻止操作背景
向 AI：点击删除按钮后显示模态确认对话框，页面变暗约 40%，用 0.3 s 淡入并略微放大。

#073 视差滚动（Parallax scrolling）：滚动时背景层比内容移动得慢
向 AI：让首屏背景以滚动距离的 0.3× 移动，形成视差滚动。

#097 逆光（Backlighting）：光源位于主体后方
向 AI：草地人像用逆光，低处太阳正对头后，发丝边缘发亮，带柔和薄雾。

#101 伦勃朗光（Rembrandt lighting）：侧上方光在背光脸颊留下亮三角
向 AI：老人肖像用伦勃朗光，从侧上方 45° 打光，背光侧脸颊留一小块三角亮区。

#121 预备动作（Anticipation）：运动前先向反方向稍稍蓄力
向 AI：按钮向右飞出前加上预备动作：先用 0.3 s 向反方向稍稍后拉并压扁，再飞出去。

#145 滚动时间轴（Timeline on scroll）：滚动时时间轴的线条随之延伸
向 AI：把公司沿革做成滚动时间轴：竖线随滚动延伸，线到达哪一年就依次显示该年内容。

#169 垂直升降镜头（Pedestal）：相机整体垂直上下平移
向 AI：保持镜头朝向不变，用垂直升降镜头从眼睛高度直线上升到约 3 m。
```

- **原文语言**：中文（摘自仓库简体中文「向 AI 提出需求的示例」，原文照录）
- **中文含义**：从 showheyohtaki/motion-prompt 的 192 条效果库里，按 8 个分类各抽 1–2 条代表性「向 AI 怎么说」例句（含编号、中文名、英文名、含义）。完整库含动态图形、镜头、UI、落地页、摄影等，每条还有动态示例。
- **用途**：不知道专业动效 / 镜头 / UI 效果叫什么时，用标准名称 + 具体参数向 AI 描述，比空泛地说“做点动画”更准。
- **使用场景**：写落地页动效、视频运镜、UI 交互动画、摄影布光提示词；或让 Claude Code / Codex 按编号改界面。
- **适用工具**：Claude Code / Codex 等（仓库提供 Agent Skill：`npx skills add showheyohtaki/motion-prompt`）；也适用于通用对话式 AI
- **需替换的变量**：每条例句里的对象（标志、卡片、人物、背景等）、时长、幅度可按需改。也可直接说「用 #032」引用画廊编号。
- **技巧与注意**：这不是把 192 条全塞进来：完整列表与动态画廊在 https://showheyohtaki.github.io/motion-prompt/ 和仓库 `packs/`。安装 Skill：`npx skills add showheyohtaki/motion-prompt`。例句来自 `packs/*/meta.json` 的 `ask.zh-Hans` 字段（与 README.zh-Hans 表格一致）。作者大滝昇平（@showheyohtaki），帖子是摸鱼巨匠转发介绍。
- **来源**：大滝昇平 / Shohei Ohtaki（@showheyohtaki）；介绍帖摸鱼巨匠（@ChatGptAstra），<https://x.com/ChatGptAstra/status/2119732495747043631>，2026-11-09
