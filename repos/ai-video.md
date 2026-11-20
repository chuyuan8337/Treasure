# AI 视频与剪辑

以下仓库整理自 Levi 卧云（@zmdsb259414）2026-10-22 的帖子：<https://x.com/zmdsb259414/status/2113140946699460933>

baocut 整理自宝玉（@dotey）2026-10-25 的帖子：<https://x.com/dotey/status/2114375050971296135>

CozyClay 整理自 AI超元域（@AISuperDomain）2026-10-25 的帖子：<https://x.com/AISuperDomain/status/2114327756532036045>

OpenMotion 整理自 Tom Huang（@tuturetom）2026-11-17 的帖子：<https://x.com/tuturetom/status/2122633782654370068>

Stars 和更新日期来自 GitHub API，查询于 2026-10-23（北京时间），更新日期按最后一次推送换算为北京时间；帖子里的 star 数是发帖时的约数，略低于现值；OpenMotion 查询于 2026-11-19（北京时间）。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | 给 Claude Code / Codex 用的视频 skill，用 Remotion 写代码出电影感产品视频，含 152 张镜头配方卡 | TypeScript | 12,991 | 2026-10-18 | Apache-2.0 | 产品宣传片、推广视频，用代码批量出片 | [@zmdsb259414 2026-10-22](https://x.com/zmdsb259414/status/2113140946699460933) | 2026-10-23（北京时间） |
| [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | 不用视频模型、纯代码做短片的风格工具箱，现有 59 种电影风格（帖子写的是 51 种） | JavaScript | 5,567 | 2026-10-22 | MIT | AI 短片、动画风格参考与复用 | [@zmdsb259414 2026-10-22](https://x.com/zmdsb259414/status/2113140946699460933) | 2026-10-23（北京时间） |
| [Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) | 15 种 MG 动效风格，成片、提示词、完整源码都公开 | Python | 1,840 | 2026-10-05 | MIT | 学习 MG 动效、照着提示词和源码拆解 | [@zmdsb259414 2026-10-22](https://x.com/zmdsb259414/status/2113140946699460933) | 2026-10-23（北京时间） |
| [mcncarl/jianying-headless](https://github.com/mcncarl/jianying-headless) | 剪映专业版（macOS）草稿的无头生成、编辑与原生导出工具，附 Agent Skill；Windows 另有 FFmpeg 导出 | Python | 3,921 | 2026-10-21 | 仅限个人非商用 | 批量生成剪映草稿、Agent 辅助剪辑 | [@zmdsb259414 2026-10-22](https://x.com/zmdsb259414/status/2113140946699460933) | 2026-10-23（北京时间） |
| [JimLiu/baocut](https://github.com/JimLiu/baocut) | 以可编辑时间线为中心的 AI 视频 Agent（桌面 App + CLI + MCP + [Skill](https://github.com/JimLiu/baocut/blob/main/skills/baocut/SKILL.md)）：转录、字幕、逐句翻译、配音、剪口播、动效图形，结果都能接着改；官网 <https://baocut.com/> | TypeScript | 1,450 | 2026-10-26 | BaoCut Community License（源码可见） | 给视频做中英双语字幕、把播客 / 音频做成带字幕的版面视频、让 Claude Code / Codex 驱动剪辑 | [@dotey 2026-10-25](https://x.com/dotey/status/2114375050971296135) | 2026-10-26（北京时间） |
| [NomaDamas/CozyClay](https://github.com/NomaDamas/CozyClay) | 浏览器里的开源 3D 视频预演（previs）工具：搭场景、用自然语言编排人物动作（自动检查碰撞、脚步滑动）、设计镜头与剪切，再导出首尾帧、灰盒参考视频和提示词交给 AI 视频模型；带 MCP Server；在线试用 <https://cozyclay.org/> | JavaScript | 1,072 | 2026-10-26 | AGPL-3.0 | 做 AI 视频前先定好站位、动作和运镜，减少“抽卡”；让 Claude Code / Cursor 通过 MCP 操控分镜 | [@AISuperDomain 2026-10-25](https://x.com/AISuperDomain/status/2114327756532036045) | 2026-10-26（北京时间） |
| [nexu-io/openmotion](https://github.com/nexu-io/openmotion) | 开源全栈 Agent 视频工作室（官方口号称 Claude Motion / CapCut 平替）：按参考视频或链接复刻成可编辑的 HTML 动效工程，换上自己的品牌和文案再导出 MP4 等；带 Motion.md、本地 Studio 和 MCP，README 写支持 22 个本地 Agent；官网 <https://open-design.ai/motion/> | TypeScript | 12,018 | 2026-11-19 | Apache-2.0 | 把参考宣传片改成自己的品牌成片；用 Claude Code / Codex / DSH 等在本地做可继续修改的动效视频 | [@tuturetom 2026-11-17](https://x.com/tuturetom/status/2122633782654370068) | 2026-11-19（北京时间） |

## 注意事项

jianying-headless 的仓库 LICENSE 为 Personal Learning and Non-Commercial Use License，只允许个人学习和非商业使用，商用前请先确认授权。它需要本机安装匹配版本的剪映（主要适配 11.5.0），不是剪映官方 SDK。

baocut 的 LICENSE 是自定义的 BaoCut Community License（GitHub 显示为 Other，源码可见而非 OSI 开源）：个人、学习、公司内部使用，以及用它做的视频等内容（包括广告、变现视频、接单剪辑）都可以商用；但商业分发软件本身、做成对外的收费服务 / 平台 / API、把代码放进商业产品，需要另谈书面授权。帖子原话是「使用 BaoCut Skill 即可做这种排版的视频（需要安装 BaoCut App 配合转录和对齐翻译）」，即只装 Skill 不够。需要 macOS 14+（Apple Silicon）或 Windows x64，另装 ffmpeg / ffprobe；Agent 功能要已登录的 Claude Code、Codex CLI 等；Windows 安装包未签名；内置的 Fish Audio S2 Pro 语音模型为研究 / 非商用许可。

CozyClay 的许可证是 AGPL-3.0-or-later（2026-08-21 以前的贡献为 GPL-3.0-or-later）：自己用、用它做视频都没问题，但修改后通过网络给别人用就必须公开对应源码。安装是 `npx cozyclay`，需要 Node.js 22.19+ 和 Chromium 浏览器，不需要 GPU、Python 或下载模型；也可以在 <https://cozyclay.org/> 直接试用。内置的 AI 动作编排要登录 ChatGPT 或自备 Anthropic / OpenAI / Gemini / MiniMax / OpenRouter 等 key；视频本身还要另外的 AI 视频模型生成。官方 npm 包和网站会发匿名使用统计（PostHog，无 cookie、不录屏），可用 `cclay telemetry off` 关闭。

OpenMotion 的仓库 LICENSE 为 Apache-2.0，仓库本体可按该许可使用；第三方代码、模板、媒体和字体保留各自许可。它是本地优先的 HTML 动效工作室，不是剪映专业版草稿导出器（那条是 jianying-headless），也不是单独的 Remotion Skill（那条是已收录的 video-shotcraft；作者在线程里致谢了它，不重复计算）。路径是 BYOA / BYOK：生图、生视频、配乐、配音要走付费模型服务，也可选 OpenDesign Go 订阅。安装 Skill（`npx skills add nexu-io/openmotion --skill openmotion`）本身不会自动装好 Studio 或连上 MCP。package.json 要求 Node.js 22.18 及以上，本地运行说明里写的是 Node.js 26.11.1；预览和导出还要 Chrome / Chromium 与 FFmpeg / FFprobe。当前 package.json 版本为 0.0.1。

宣传与目录的差别（2026-11-19 查看发布目录 catalog.json）：「还原度超 95%」和「14 天 47 万行代码」只出现在原帖，README 没有同样口径，前者未验证，后者未统计行数（仓库 2026-05-11 已创建）。原帖「152+设计系统」在线程里改口为「152+ Brandkit」；发布目录里模板 287 条（少于宣传的 300+）、Skills 104 项、品牌名 100 个，未在同一份目录里数到 152 个 Brandkit。README 写 22 个本地 Agent（帖子写 20+）。复刻参考片时应使用自己拥有或获准的品牌与素材，不要把他人的影视作品或商标当成可任意改编、商用的模板。帖子与线程附有多条演示视频，收录时未观看。
