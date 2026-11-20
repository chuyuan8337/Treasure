# Treasure

个人长期收集的好资源（工具、开源仓库、文章）。按资源类型分目录，同一类型里按主题各写一个 Markdown 文件；之后要加条目，在对应文件的表里补一行即可。

开源仓库放在 [`repos/`](repos/)，网站类工具放在 [`tools/`](tools/)，提示词放在 [`prompts/`](prompts/)（原文照录，附中文用途和使用场景）。之后如果收入文章，按同样方式增加 `articles/`，并补进下面的索引。

## 收录说明

共 31 个开源仓库和 2 个在线工具：8 个仓库整理自 Levi 卧云（@zmdsb259414）2026-10-22 的帖子，2 个仓库和 1 个网站整理自风清扬（@hassanyehiaa）2026-10-22 的帖子，1 个仓库整理自丹丹爱学习（@dandanetha）2026-10-24 的帖子，1 个仓库整理自宝玉（@dotey）2026-10-25 的帖子，1 个仓库整理自 Elaya（@elayadesigns）2026-10-25 的帖子，1 个仓库整理自 AI超元域（@AISuperDomain）2026-10-25 的帖子，1 个（earshot）是用户自行补充的。另有 1 个在线工具（IPdodo）整理自霍舟（@realhoimusk）2026-10-24 的帖子。另有 7 个 UI 组件库整理自摸鱼巨匠（@ChatGptAstra）2026-11-08 的帖子。另有 1 个动效提示词库（motion-prompt）整理自同作者 2026-11-09 的帖子。另有 1 个 UI 组件库（Astryx）整理自 awe0（@awe0_io）2026-11-08 的帖子。另有 1 个设计 Skill（unslop）整理自 별똥별（@stellargent_lab）2026-11-10 的帖子。另有 1 个游戏精灵 Skill（agent-sprite-forge）是用户自行补充的。另有 1 个 UI 组件库（Fluid / useFluid/fluidui）整理自 Willian Figueiredo（@willradoux）2026-11-14 的帖子。另有 1 个交互线稿插画库（Hairline / lucasmarkes/hairline）整理自 Viking（@vikingmute）2026-11-14 的帖子。另有 1 个全栈 Agent 视频工作室（OpenMotion / nexu-io/openmotion）整理自 Tom Huang（@tuturetom）2026-11-17 的帖子。另有 1 个构造线插画 Skill（Plotter / pasqualevitiello/plotter）整理自 sundyme 2026-11-19 的帖子。另有 1 个像素特效库（pixelfx / patch-gg/pixelfx）整理自黑箱之外（@BeyondTheBoxCN）2026-11-19 的帖子。均已核实，各条的统计核对日期写在分类文件里。

原帖：<https://x.com/zmdsb259414/status/2113140946699460933>

风清扬的帖子：<https://x.com/hassanyehiaa/status/2113246930507899163>。作者宣布他的免费中小学知识图谱新增初中物理，并公开另一个本地合成视频 BGM 的仓库。知识图谱写在 [教育与知识图谱](repos/education.md)，BGM 写在 [AI 音频](repos/ai-audio.md)，在线网站写在 [教育工具](tools/education.md)。

作者把自己 star 过的 AI 视频、AI 3D、Three.js 相关仓库整理成一份清单，共 8 个。作者在评论区的回复里没有补充其他仓库。这 8 个写在 [AI 3D 与 Three.js](repos/ai-3d.md) 和 [AI 视频与剪辑](repos/ai-video.md)。earshot 写在 [AI 音频](repos/ai-audio.md)，不在原帖清单里。

Stars 和更新日期来自 GitHub API，查询于 2026-10-23（北京时间），更新日期按最后一次推送换算为北京时间；帖子里的 star 数是发帖时的约数，略低于现值。各分类文件逐条写了来源和统计核对日期。

提示词：1 条整理自サークルきなこ棒（@circlekinakoboo）2026-10-24 的帖子 <https://x.com/circlekinakoboo/status/2113824297777308119>，作者分享了一句压制 GPT-image2.5 生成图里细碎纹理、减少“AI 感”的提示词。

视频提示词：2 条整理自 iX（@iX00AI）的帖子。p002 来自 2026-10-25 的 <https://x.com/iX00AI/status/2114305325683937294>（用 TOPVIEW T1 生成的 2003 年 DV 家庭录像风“女高中生大战巨型怪物”短片）；p003 来自它引用的 2026-10-23 推广帖 <https://x.com/iX00AI/status/2113462863381868999>（同一份提示词对比 TOPVIEW T1 和 Seedance 2.5）。两条都是作者与 TOPVIEW 合作的推广内容，效果以作者自己的视频为准。

视频提示词 p004–p005：一套“孟菲斯微缩世界”代码动画提示词，不用视频模型，让 AI 用 Canvas 逐帧画、无头 Chrome 导出、ffmpeg 合成，配乐也用代码生成。p004 是 Eian（@EianLu）2026-10-26 发的通用模板 <https://x.com/EianLu/status/2114695987424063730>；p005 是 Regen（@huqinyiyayuguan）2026-10-26 用这套模板写的北京东三环央视大楼街景版 <https://x.com/huqinyiyayuguan/status/2114717363736400279>。

视频提示词 p007：Lemomo（@lemomo_ai）2026-11-17 的帖子 <https://x.com/lemomo_ai/status/2122547781592117459>，用同一组雨夜素材示范 7 种后期滤镜（黑柔、变形宽银幕拉丝、留银、星光镜、烟草渐变镜、光晕 + 16 毫米、红滤镜黑白），并说明滤镜是情绪放大器，只要向 agent 讲清情绪和搭配的滤镜即可。作者在回复里确认这是同一段素材额外加的后期（不是生成时指定），后期 Agent 就可以加，还可以调色，尤其是 Blender；也提到 Codex 能做这类剪辑。这不是视频模型提示词，也不是同一作者已收录的 lemo-opuscar 风格库里的条目。帖子附 85 秒视频，收录时未观看。

丹丹爱学习（@dandanetha）2026-10-24 的帖子 <https://x.com/dandanetha/status/2113852735330365607>：推荐 Agent Reach，让 Claude Code、Cursor、Codex 等 Agent 能搜 X、读小红书、看 B 站字幕等。写在 [AI Agent 工具](repos/ai-agent-tools.md)。

宝玉（@dotey）2026-10-25 的帖子 <https://x.com/dotey/status/2114375050971296135>：回答网友“带实时翻译的视频是怎么做出来的”，用 BaoCut Skill 配合 BaoCut App（转录和对齐翻译）就能做这种双语字幕排版的视频，音频也可以。写在 [AI 视频与剪辑](repos/ai-video.md)。

Elaya（@elayadesigns）2026-10-25 的帖子 <https://x.com/elayadesigns/status/2114049200749175174>：展示两个月内用 Higgsfield、Claude、Cursor 加自制 AI 设计师 Skill 做的一批落地页，并开源了这个 Skill。写在 [AI 设计](repos/ai-design.md)。

AI超元域（@AISuperDomain）2026-10-25 的帖子 <https://x.com/AISuperDomain/status/2114327756532036045>：介绍开源 3D 视频预演工具 CozyClay，生成 AI 视频前先在浏览器里把场景、人物动作和镜头设计好，再把首尾帧、灰盒参考视频和提示词交给视频模型。写在 [AI 视频与剪辑](repos/ai-video.md)。

霍舟（@realhoimusk）2026-10-24 的帖子 <https://x.com/realhoimusk/status/2113840831484596534>：提醒做推特一定要用住宅 IP 以免封号，推荐自己在用的 IPdodo 住宅 IP。它是闭源收费的商业网络服务、不是 AI 工具，单独写在 [网络与账号环境](tools/network.md)。帖子里的链接带作者邀请码，防封效果是作者的说法。

摸鱼巨匠（@ChatGptAstra）2026-11-08 的帖子 <https://x.com/ChatGptAstra/status/2119349702688641177>：推荐 7 个网页 / 移动端 UI 组件库（Looseleaf、Rare UI、ExpoKit、goopUI、beUI、Sketchbook UI、AffectUI）。现有「AI 设计」是 Skill，这些是可安装组件库，单独写在 [UI 组件库](repos/ui-components.md)。作者后来另发帖介绍 motion-prompt，未计入本条。

摸鱼巨匠（@ChatGptAstra）2026-11-09 的帖子 <https://x.com/ChatGptAstra/status/2119732495747043631>：介绍开源项目 motion-prompt（大滝昇平 @showheyohtaki），192 个带专业名称的动效 / 镜头 / UI / 落地页 / 摄影效果库，可 Copy Prompt，也可 `npx skills add showheyohtaki/motion-prompt`。写在 [动效与提示词库](repos/motion-prompt.md)；代表性例句写在 [动效与创意词汇](prompts/motion-vocabulary.md)。

awe0（@awe0_io）2026-11-08 的帖子 <https://x.com/awe0_io/status/2119354093458395284>：介绍 Meta 开源设计系统 Astryx（MIT、Beta，150+ 组件，CLI / 文档站 MCP 方便 AI Agent）。写在 [UI 组件库](repos/ui-components.md)。

별똥별（@stellargent_lab）2026-11-10 的帖子 <https://x.com/stellargent_lab/status/2119919314497364236>：介绍设计 Skill unslop（仓库 https://github.com/heydamir/unslop，作者 Damir Sokolovsky @heydamir），把 vibe coding 界面去掉“AI 味”。写在 [AI 设计](repos/ai-design.md)。

用户自行补充的仓库 <https://github.com/0x0funky/agent-sprite-forge>：Agent Sprite Forge，给 Claude Code / Codex / Grok 用的 Agent Skill，用一张批准的原画生成整套可进游戏的 2D 精灵、地图和像素风。写在 [AI 游戏精灵与像素美术](repos/ai-game-sprites.md)。

Willian Figueiredo（@willradoux）2026-11-14 的帖子 <https://x.com/willradoux/status/2121444548681277723>：开源发布 Fluid，一套带品牌感的 React 动效组件库（引擎、可拷贝组件、可选 Agent Skill，也可逐帧录视频）。写在 [UI 组件库](repos/ui-components.md)。官网 <https://fluidui.willradoux.com>，仓库 <https://github.com/useFluid/fluidui>。

Viking（@vikingmute）2026-11-14 的帖子 <https://x.com/vikingmute/status/2121607129547043219>：推荐 Hairline（作者 Lucas Marques），33 个会响应指针的等距线稿 SVG 插画，可调 intensity。写在 [交互线稿插画](repos/line-figures.md)。官网 <https://hairline.lucasmarkes.com>，仓库 <https://github.com/lucasmarkes/hairline>。发帖人不是项目作者。

Tom Huang（@tuturetom）2026-11-17 的帖子 <https://x.com/tuturetom/status/2122633782654370068>：宣布开源 OpenMotion，自称 Claude Motion / 剪映平替，可用本地 Agent 按参考视频复刻可编辑的动效工程。仓库 https://github.com/nexu-io/openmotion ，官网 https://open-design.ai/motion/ 。写在 [AI 视频与剪辑](repos/ai-video.md)。宣传数字与发布目录的差异、第三方品牌素材和付费模型依赖见该文件注意事项。

sundyme 2026-11-19 的帖子 <https://x.com/sundyme/status/2123284282009649414>：推荐 Plotter（作者 Pasquale Vitiello @pacovitiello），用 Claude Code / Codex 画可编辑的单色构造线 SVG，也可做成 HTML 动画。官网 https://plotter.pasqualevitiello.com/ ，仓库 https://github.com/pasqualevitiello/plotter 。发帖人不是项目作者。写在 [交互线稿插画](repos/line-figures.md)。

黑箱之外（@BeyondTheBoxCN）2026-11-19 的帖子 <https://x.com/BeyondTheBoxCN/status/2123400914149298423>：介绍 pixelfx，244 种用代码生成的像素特效，可预览并导出精灵表，带 Claude Code Skill。仓库 https://github.com/patch-gg/pixelfx 。发帖人不是项目作者。它此前只在 agent-sprite-forge 注意事项里作为可选依赖出现，现单独收录，不重复计条。写在 [AI 游戏精灵与像素美术](repos/ai-game-sprites.md)。

## 索引

### 开源仓库

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| AI 3D 与 Three.js | [repos/ai-3d.md](repos/ai-3d.md) | 4 |
| AI 视频与剪辑 | [repos/ai-video.md](repos/ai-video.md) | 7 |
| AI 音频 | [repos/ai-audio.md](repos/ai-audio.md) | 2 |
| 教育与知识图谱 | [repos/education.md](repos/education.md) | 1 |
| AI Agent 工具 | [repos/ai-agent-tools.md](repos/ai-agent-tools.md) | 1 |
| AI 设计 | [repos/ai-design.md](repos/ai-design.md) | 2 |
| UI 组件库 | [repos/ui-components.md](repos/ui-components.md) | 9 |
| 动效与提示词库 | [repos/motion-prompt.md](repos/motion-prompt.md) | 1 |
| AI 游戏精灵与像素美术 | [repos/ai-game-sprites.md](repos/ai-game-sprites.md) | 2 |
| 交互线稿插画 | [repos/line-figures.md](repos/line-figures.md) | 2 |

### 工具

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| 教育工具 | [tools/education.md](tools/education.md) | 1 |
| 网络与账号环境（非 AI · 商业服务） | [tools/network.md](tools/network.md) | 1 |

### 提示词

| 分类 | 文件 | 条目 |
| --- | --- | --- |
| 图像生成 | [prompts/image-generation.md](prompts/image-generation.md) | 1 |
| 视频生成 | [prompts/video-generation.md](prompts/video-generation.md) | 5 |
| 动效与创意词汇 | [prompts/motion-vocabulary.md](prompts/motion-vocabulary.md) | 1 |

使用限制写在对应文件的「注意事项」里：jianying-headless 只允许个人学习和非商业使用，并需要本机安装主要适配 11.5.0 的剪映；earshot 可选的 `llm` 命令会把音频上传到 Gemini。cn-math-taxonomy 为 CC BY-NC 4.0（不能商用）且是未经教师审核的 AI 初稿；timeline-bgm 没有声明许可证。Agent-Reach 会复用浏览器里的登录（建议用小号），X 等渠道为实验状态，且只能从 GitHub 的 install.md 安装（PyPI 同名包不是本项目）。baocut 为自定义的 BaoCut Community License：用它做的内容可商用，但商业分发软件或做成对外收费服务需另行授权。ai-design-skills 为 MIT，但作者承认部分内容源自 taste-skill、尚待补署名。CozyClay 为 AGPL-3.0（修改后对外提供网络服务须公开源码），且默认发送匿名使用统计（可关闭）。IPdodo 是收费商业服务，帖子链接带作者邀请码，需自备海外网络才能使用，“住宅 IP 防封号”未经核实。Rare UI 为 MIT + Commons Clause + 署名（不可单独再分发组件）；ExpoKit / affectUI 另有付费 Pro；goopUI 仍为 pre-alpha（目前主要 Vue）。Astryx 为 Beta，需 React 19+；图表包仅有 @canary。unslop 为 CC BY 4.0（须署名）；配图与故事视频依赖可选的付费图像服务 / Playwright+ffmpeg。agent-sprite-forge 为 MIT，但出图 / 出视频依赖付费 API 或 Codex / Grok 订阅额度；Godot / Aseprite / LDtk 等编辑器导入尚未在编辑器里验证。Fluid（useFluid/fluidui）为 MIT，刚发布（npm 0.1.2）；组件拷进项目后不会自动更新；录视频需要 Chrome/Edge、playwright-core 和 ffmpeg。Hairline 为 MIT；随包装的是 33 个 figure，图鉴里的 Vercel / Mastra / Notion 致敬稿不在包装内且标志归其所有者；与 Linear 没有隶属关系（仅作感觉参考）。OpenMotion 为 Apache-2.0，但第三方模板 / 媒体 / 字体保留原许可；生图与生视频等依赖 BYOK 或 OpenDesign Go；「95% 还原度」「14 天 47 万行」「152+ Brandkit / 设计系统」等宣传数字未全部被 README 或发布目录证实。Plotter 为 MIT（抽取历史曾有 AGPL 记录；Cal Sans 为 OFL-1.1），Skill 独立于官网，画图消耗 Claude Code / Codex 额度。pixelfx 代码与特效为 MIT，但画廊字体 Patch Pixel 不在该许可内；发到 Patch.gg 是可选功能。
