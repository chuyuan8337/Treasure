# Treasure

个人长期收集的好资源（工具、开源仓库、文章）。按资源类型分目录，同一类型里按主题各写一个 Markdown 文件；之后要加条目，在对应文件的表里补一行即可。

开源仓库放在 [`repos/`](repos/)，网站类工具放在 [`tools/`](tools/)，提示词放在 [`prompts/`](prompts/)（原文照录，附中文用途和使用场景）。之后如果收入文章，按同样方式增加 `articles/`，并补进下面的索引。

## 收录说明

共 15 个开源仓库和 1 个在线工具：8 个仓库整理自 Levi 卧云（@zmdsb259414）2026-10-22 的帖子，2 个仓库和 1 个网站整理自风清扬（@hassanyehiaa）2026-10-22 的帖子，1 个仓库整理自丹丹爱学习（@dandanetha）2026-10-24 的帖子，1 个仓库整理自宝玉（@dotey）2026-10-25 的帖子，1 个仓库整理自 Elaya（@elayadesigns）2026-10-25 的帖子，1 个仓库整理自 AI超元域（@AISuperDomain）2026-10-25 的帖子，1 个（earshot）是用户自行补充的。均已核实，各条的统计核对日期写在分类文件里。

原帖：<https://x.com/zmdsb259414/status/2113140946699460933>

风清扬的帖子：<https://x.com/hassanyehiaa/status/2113246930507899163>。作者宣布他的免费中小学知识图谱新增初中物理，并公开另一个本地合成视频 BGM 的仓库。知识图谱写在 [教育与知识图谱](repos/education.md)，BGM 写在 [AI 音频](repos/ai-audio.md)，在线网站写在 [教育工具](tools/education.md)。

作者把自己 star 过的 AI 视频、AI 3D、Three.js 相关仓库整理成一份清单，共 8 个。作者在评论区的回复里没有补充其他仓库。这 8 个写在 [AI 3D 与 Three.js](repos/ai-3d.md) 和 [AI 视频与剪辑](repos/ai-video.md)。earshot 写在 [AI 音频](repos/ai-audio.md)，不在原帖清单里。

Stars 和更新日期来自 GitHub API，查询于 2026-10-23（北京时间），更新日期按最后一次推送换算为北京时间；帖子里的 star 数是发帖时的约数，略低于现值。各分类文件逐条写了来源和统计核对日期。

提示词：1 条整理自サークルきなこ棒（@circlekinakoboo）2026-10-24 的帖子 <https://x.com/circlekinakoboo/status/2113824297777308119>，作者分享了一句压制 GPT-image2.5 生成图里细碎纹理、减少“AI 感”的提示词。

丹丹爱学习（@dandanetha）2026-10-24 的帖子 <https://x.com/dandanetha/status/2113852735330365607>：推荐 Agent Reach，让 Claude Code、Cursor、Codex 等 Agent 能搜 X、读小红书、看 B 站字幕等。写在 [AI Agent 工具](repos/ai-agent-tools.md)。

宝玉（@dotey）2026-10-25 的帖子 <https://x.com/dotey/status/2114375050971296135>：回答网友“带实时翻译的视频是怎么做出来的”，用 BaoCut Skill 配合 BaoCut App（转录和对齐翻译）就能做这种双语字幕排版的视频，音频也可以。写在 [AI 视频与剪辑](repos/ai-video.md)。

Elaya（@elayadesigns）2026-10-25 的帖子 <https://x.com/elayadesigns/status/2114049200749175174>：展示两个月内用 Higgsfield、Claude、Cursor 加自制 AI 设计师 Skill 做的一批落地页，并开源了这个 Skill。写在 [AI 设计](repos/ai-design.md)。

AI超元域（@AISuperDomain）2026-10-25 的帖子 <https://x.com/AISuperDomain/status/2114327756532036045>：介绍开源 3D 视频预演工具 CozyClay，生成 AI 视频前先在浏览器里把场景、人物动作和镜头设计好，再把首尾帧、灰盒参考视频和提示词交给视频模型。写在 [AI 视频与剪辑](repos/ai-video.md)。

## 索引

### 开源仓库

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| AI 3D 与 Three.js | [repos/ai-3d.md](repos/ai-3d.md) | 4 |
| AI 视频与剪辑 | [repos/ai-video.md](repos/ai-video.md) | 6 |
| AI 音频 | [repos/ai-audio.md](repos/ai-audio.md) | 2 |
| 教育与知识图谱 | [repos/education.md](repos/education.md) | 1 |
| AI Agent 工具 | [repos/ai-agent-tools.md](repos/ai-agent-tools.md) | 1 |
| AI 设计 | [repos/ai-design.md](repos/ai-design.md) | 1 |

### 工具

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| 教育工具 | [tools/education.md](tools/education.md) | 1 |

### 提示词

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| 图像生成 | [prompts/image-generation.md](prompts/image-generation.md) | 1 |

使用限制写在对应文件的「注意事项」里：jianying-headless 只允许个人学习和非商业使用，并需要本机安装主要适配 11.5.0 的剪映；earshot 可选的 `llm` 命令会把音频上传到 Gemini。cn-math-taxonomy 为 CC BY-NC 4.0（不能商用）且是未经教师审核的 AI 初稿；timeline-bgm 没有声明许可证。Agent-Reach 会复用浏览器里的登录（建议用小号），X 等渠道为实验状态，且只能从 GitHub 的 install.md 安装（PyPI 同名包不是本项目）。baocut 为自定义的 BaoCut Community License：用它做的内容可商用，但商业分发软件或做成对外收费服务需另行授权。ai-design-skills 为 MIT，但作者承认部分内容源自 taste-skill、尚待补署名。CozyClay 为 AGPL-3.0（修改后对外提供网络服务须公开源码），且默认发送匿名使用统计（可关闭）。
