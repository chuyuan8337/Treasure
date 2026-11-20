# AI 设计

以下仓库整理自：

- Elaya（@elayadesigns）2026-10-25 的帖子：<https://x.com/elayadesigns/status/2114049200749175174>
- 별똥별（@stellargent_lab）2026-11-10 的帖子：<https://x.com/stellargent_lab/status/2119919314497364236>（仓库由作者回复给出）

Stars 和更新日期来自 GitHub API；`ai-design-skills` 查询于 2026-10-26（北京时间），`unslop` 查询于 2026-11-10（北京时间）。更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [elayadesign/ai-design-skills](https://github.com/elayadesign/ai-design-skills) | 给 Claude Code / Cursor / Codex 等 AI 编程工具用的设计 Skill 合集：`landing-page-design`（从需求询问、页面结构、转化文案到完整视觉规范）和 `design-to-motion`（把静态设计做成循环动画，导出 MP4 / GIF） | Markdown（无代码） | 5,373 | 2026-10-25 | MIT | 让 AI 做出不平庸的落地页 / 营销站、给设计稿做展示动画 | [@elayadesigns 2026-10-25](https://x.com/elayadesigns/status/2114049200749175174) | 2026-10-26（北京时间） |
| [heydamir/unslop](https://github.com/heydamir/unslop) | 给 Claude Code / Codex / Google Antigravity 用的设计 Skill：先找出紫色渐变、光晕、emoji 标签、喊口号文案、间距不均这类“AI 味”，再按产品定方向、分轮次改成更像设计师过稿的界面 | JavaScript | 12,957 | 2026-11-09 | CC BY 4.0 | 把 vibe coding 出来的仪表盘 / 落地页 / 在线站点去掉套模板感；支持 React、Vue、普通 HTML，也可给一个线上链接 | [@stellargent_lab 2026-11-10](https://x.com/stellargent_lab/status/2119919314497364236) | 2026-11-10（北京时间） |

安装：Claude Code 把 `skills/<skill-name>` 文件夹拷进 `.claude/skills/`；Cursor 把 `SKILL.md` 放进 `.cursor/rules/`；Codex 写进 `AGENTS.md`。改造已有网站用作者另一个仓库 [elayadesign/redesign-skill](https://github.com/elayadesign/redesign-skill)（未单独核实，未计入总数）。

unslop 安装（摘自仓库 README）：Claude Code 把 `skills/unslop` 拷进 `~/.claude/skills/` 或项目 `.claude/skills/`；Codex 可用 `$skill-installer install https://github.com/heydamir/unslop/tree/main/skills/unslop`，或拷进 `~/.agents/skills/`；Google Antigravity 拷进 `~/.gemini/antigravity/skills/`。使用：`/unslop …`（Claude Code）或 `$unslop …`（Codex）。

## 注意事项

- 评论区有人（@LexnLin）要求为 taste-skill 署名，作者回复承认部分内容来自调研时没追溯到 taste-skill，说会在两个仓库加署名并重写重叠部分；2026-10-26 查看时 README 的致谢里还没有 taste-skill（只列了 design-to-motion 借鉴的 emilkowalski/skills、Owl-Listener/designer-skills、dylantarre/animation-principles）。
- 帖子里的落地页还用到了付费 AI 创作平台 Higgsfield，Skill 本身不包含它。
- **unslop（heydamir/unslop）**：CC BY 4.0，商用可以，但须署名 Damir Sokolovsky（@heydamir）并链接回该仓库。生成配图需另接付费图像服务（fal、Replicate、OpenAI images、Higgsfield 等），每次生成前会询问。做不到 10 秒的改造过程方视频需 Playwright Chromium + 系统 ffmpeg。作者另有付费代改服务 https://heydamir.design/unslop ，与开源 Skill 分开。
