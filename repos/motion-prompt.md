# 动效与提示词库

以下仓库整理自摸鱼巨匠（@ChatGptAstra）2026-11-09 的帖子：<https://x.com/ChatGptAstra/status/2119732495747043631>

Stars 和更新日期来自 GitHub API，查询于 2026-11-10（北京时间），更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [showheyohtaki/motion-prompt](https://github.com/showheyohtaki/motion-prompt) | 192 个带专业名称的动效 / 镜头 / UI / 落地页 / 摄影效果库：每个有动态示例、含义和可复制的「向 AI 怎么说」例句；可作 Agent Skill（`npx skills add`） | JavaScript | 1,587 | 2026-10-29 | MIT | 不知道专业动效叫什么时翻一览、点 Copy Prompt 让 AI 实现；或让 Agent 按编号改界面 / 出片 | [@ChatGptAstra 2026-11-09](https://x.com/ChatGptAstra/status/2119732495747043631) | 2026-11-10（北京时间） |

- 画廊：<https://showheyohtaki.github.io/motion-prompt/>
- 名称列表：仓库 [`packs/`](https://github.com/showheyohtaki/motion-prompt/tree/main/packs)（英 / 日 / 西 / 简中 / 繁中）
- Agent Skill：`npx skills add showheyohtaki/motion-prompt`
- 作者：大滝昇平 / Shohei Ohtaki（@showheyohtaki）

八组 packs（各 24 条，共 192）：`motion`、`camera`、`ui`、`lp`、`photo`、`motion2`、`lp2`、`camera2`。

## 注意事项

- 这是「专业名称 + 动态示例 + 例句」词汇库，不是 UI 组件库；演示动画是无依赖 Canvas 2D。
- 提示词合集只摘了代表性「向 AI」例句（见 `prompts/motion-vocabulary.md`），完整 192 条以仓库 / 画廊为准。
- 仓库另有 `make-your-own/`：用来为自己的领域生成同类词库（需 Playwright、ffmpeg）。
