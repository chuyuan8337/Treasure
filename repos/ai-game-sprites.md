# AI 游戏精灵与像素美术

以下仓库由用户自行补充：<https://github.com/0x0funky/agent-sprite-forge>

pixelfx 整理自黑箱之外（@BeyondTheBoxCN）2026-11-19 的帖子：<https://x.com/BeyondTheBoxCN/status/2123400914149298423>。发帖人不是作者。

Stars 和更新日期来自 GitHub API；agent-sprite-forge 查询于 2026-11-13（北京时间），pixelfx 查询于 2026-11-20（北京时间）。更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [0x0funky/agent-sprite-forge](https://github.com/0x0funky/agent-sprite-forge) | 给 Claude Code（插件）、Codex 和 Grok 用的 Agent Skill：先批准一张角色原画，再为每个动作各生成一段图生视频，经抠图、对位、挑循环和后期后导出透明 PNG 帧、GIF 和精灵表，可打包给 Godot、Aseprite 或网页游戏；也支持地图，以及 hibit / pixel looks 两种像素风 | Python | 5,664 | 2026-11-13 | MIT | 做 2D 游戏时让 Agent 从一句角色描述产出整套动作精灵和地图；或把已有原画做成可循环的走、跑、攻击等动作 | 用户自行补充 | 2026-11-13（北京时间） |
| [patch-gg/pixelfx](https://github.com/patch-gg/pixelfx) | 244 种用 JavaScript 代码生成的像素特效（21 个分类）：可在画布上实时播放、改色和镜像，也可导出精灵表和 Aseprite 风格 JSON；另有 Claude Code Skill 辅助制作新特效；画廊 <https://patch-gg.github.io/pixelfx/> | JavaScript | 8,318 | 2026-11-13 | MIT | 做像素游戏时直接用现成特效，或导出后放进 Godot / Unity 等引擎；也可让 Agent 按同一套方法做新特效 | [@BeyondTheBoxCN 2026-11-19](https://x.com/BeyondTheBoxCN/status/2123400914149298423) | 2026-11-20（北京时间） |

- 安装（摘自仓库 README）：Claude Code 用 `claude plugin marketplace add 0x0funky/agent-sprite-forge --sparse .claude-plugin skills`，再 `claude plugin install agent-sprite-forge@agent-sprite-forge`，并 `python -m pip install "numpy>=1.26" "Pillow>=10.1" "scipy>=1.11"`。Codex / Grok：clone 仓库后 `python -m pip install -r requirements.txt`，再 `python tools/install_skills.py --apply --host codex`（Grok 把 host 改成 `grok`）。视频需要 ffmpeg 5.1+。五个 skill 文件夹要放在一起。
- 当前 CHANGELOG 版本：0.6.0（2026-11-13）。内含 skills：`generate2dsprite`、`video2dsprite`、`generate2dmap`、`generate2dmedia`、`codeart2d`。
- 多语言 README：英文、繁体中文、简体中文、日本語、한국어。

## 注意事项

- **Skill 本身 MIT 免费，出图 / 出视频要另付模型费用或消耗订阅额度。** 路径顺序：已配置的 API key（OpenAI、Gemini、xAI、BytePlus ModelArk、fal.ai）→ 已登录的 Codex CLI（`image_gen`）或 Grok CLI → 最后手段才是代码绘制（codeart2d）。配置了 key 即视为同意调用，不再逐次询问。默认没有花费上限，要用 `--budget-usd`、`--max-calls` 或 `FORGE_MAX_PAID_REQUESTS` 自己设。Key 放环境变量或用户配置文件（Linux / macOS：`~/.config/agent-sprite-forge/config.json`），不要放进项目。
- **依赖：** Python 3.10+；`requirements.txt` 为 numpy>=1.26、Pillow>=10.1、scipy>=1.11（scipy 只是加速，没有时可用纯 numpy）。做视频、精灵套装和打包还要 PATH 上的 ffmpeg 5.1+（需 libvpx-vp9 和 libx264）。codeart2d 的 SVG 栅格化另装 `requirements-codeart.txt`（resvg-py）。可选 hibit 特效路径要自行 clone 独立的 MIT 项目 [pixelfx](https://github.com/patch-gg/pixelfx)，本仓库未内置。pixelfx 现已作为独立条目收录，不重复计条。
- **编辑器导入尚未验证。** README 写明 0.4.0 的 Godot、LDtk、Aseprite 导出还没有人在编辑器里打开过（只做了解析级往返；Tiled 导出按重渲验证）。`docs/known-limitations.md` 标题仍写 0.4.0，而当前发布已是 0.6.0。
- **测试覆盖。** 开发与测量主要在 Windows 11；文档写 Linux / macOS 以及 Pillow 10.1 / numpy 1.26 最低版本的测试套件尚未跑过。数值 QA 不代替肉眼检查解剖和动作，要由 Agent 看 review 图、由人批准原画。图生视频模型在快速肢体和跳跃上容易跑偏，跑、跳动作预期要重拍。
- **生成素材授权。** MIT 只覆盖仓库的代码和文档，不覆盖用它生成的图和视频；后者受各模型服务条款约束。README 提醒不要描摹或提示你不拥有的角色；商用请用原创角色或你有权使用的 IP，并核对各服务商条款。
- 没有独立官网（GitHub `homepage` 为空）。2026-11-13 查看时有 14 个未关闭 issue、550 个 fork。
- **pixelfx 的发帖人不是作者。** 黑箱之外（@BeyondTheBoxCN）是推荐者。项目由 Patch（组织 patch-gg）维护。LICENSE 版权行：Copyright (c) 2026 Patch 与 Copyright (c) 2026 Hugo Duprez。代码和特效 MIT，可商用。`NOTICE.md`：部分核心/特效改编自 Hugo Duprez / Sprite Fusion 以及 Hollow Crown（均为 MIT）；画廊字体 Patch Pixel 不在仓库 MIT 范围内。
- **pixelfx 的用法。** 浏览器游戏可直接引用代码（无额外运行时依赖），`npm i github:patch-gg/pixelfx` 或拷贝 `src/core` 与所需特效。`node tools/render.mjs 效果编号 --sheet` 导出透明 PNG 精灵表，以及带帧区域、时长和 pivot 的 Aseprite 风格 JSON；`node tools/sheets.mjs` 可导出整个库。README 写可用 `palette` 改色，不必改特效源码。Claude Code Skill：`/plugin marketplace add patch-gg/pixelfx`，再 `/plugin install pixelfx@pixelfx`，或拷贝 `skills/pixelfx`。描述与 README / `docs/CATALOG.md` 均写 244 种特效、21 个分类。把作品发到 [Patch.gg](https://patch.gg) 是可选的，发布需要在 Windows 上打开 Patch Desktop，与使用特效库本身无关。画廊：<https://patch-gg.github.io/pixelfx/> 。帖内 52 秒视频本次未观看。2026-11-20 查看时 Stars 8,318、fork 1,083、15 个未关闭 issue。
