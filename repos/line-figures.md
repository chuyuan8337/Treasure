# 交互线稿插画

以下仓库整理自 Viking（@vikingmute）2026-11-14 的帖子：<https://x.com/vikingmute/status/2121607129547043219>

发帖人不是项目作者。项目作者是 Lucas Marques（GitHub [lucasmarkes](https://github.com/lucasmarkes)，X [@lucasmarkes__](https://x.com/lucasmarkes__)）。

Plotter 整理自 sundyme 2026-11-19 的帖子：<https://x.com/sundyme/status/2123284282009649414>。发帖人不是作者，作者是 Pasquale Vitiello（@pacovitiello）。

Stars 和更新日期来自 GitHub API；Hairline 查询于 2026-11-15（北京时间），Plotter 查询于 2026-11-20（北京时间）。更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [lucasmarkes/hairline](https://github.com/lucasmarkes/hairline) | 33 个等距线稿 SVG 插画（figure），鼠标靠近会跟手反应，可用 intensity（0 到 1）调节强度；零依赖，支持 React 或纯 DOM，也可走 shadcn 注册表；另有 `/hairline-create` 和 `/hairline-adopt` 两个可选 Agent Skill，用来自画或从已有 SVG 生成 | TypeScript | 3,867 | 2026-11-14 | MIT | 给产品页、空状态或小彩蛋加有手感的线稿插画；或让 Agent 按同一套规则画出自己的 figure | [@vikingmute 2026-11-14](https://x.com/vikingmute/status/2121607129547043219) | 2026-11-15（北京时间） |
| [pasqualevitiello/plotter](https://github.com/pasqualevitiello/plotter) | 给 Claude Code / Codex 用的 Agent Skill 和视觉语法：按简报画出可编辑的单色构造线（blueprint）SVG 插画，也可把画好的图做成带静态回退的独立 HTML 动画；官网有图鉴和语法说明 | TypeScript | 194 | 2026-11-16 | MIT | 给产品页、空状态、界面说明或系统文档画能改路径和文字的配图 | [@sundyme 2026-11-19](https://x.com/sundyme/status/2123284282009649414) | 2026-11-20（北京时间） |

- 官网 / 图鉴：<https://hairline.lucasmarkes.com> 、<https://hairline.lucasmarkes.com/figures>
- 安装（摘自 README / 文档）：`npm i @lucasmarkes/hairline`；或 `npx shadcn@latest add https://hairline.lucasmarkes.com/r/hairline.json`
- Skill：`npx skills add lucasmarkes/hairline`，然后 `/hairline-create <idea>` 或 `/hairline-adopt <file.svg>`
- 当前发版：npm / CHANGELOG / 官网均为 0.5.1（2026-10-14）。文档写全套 33 个 figure 合计约 63.5 kB gzipped，只导入一个则只带上那一个。
- 33 个 figure 按主题分 8 架（与官网图鉴一致，已按 README 表核对）：Interfaces 1、Data 3、Machines 3、Devices 3、Coding 6、Security 3、Connectivity 6、Empty 8。
- Plotter 官网：<https://plotter.pasqualevitiello.com/> ；图鉴：<https://plotter.pasqualevitiello.com/illustrations> ；安装说明：<https://plotter.pasqualevitiello.com/docs/installation>
- Plotter 安装（摘自 README / 安装页）：下载 <https://plotter.pasqualevitiello.com/plotter/downloads/plotter.zip> 或从仓库拷贝 `skills/plotter`，放到 `~/.claude/skills/plotter` 或 `~/.codex/skills/plotter`，并保持 `SKILL.md`、`agents/`、`assets/`、`references/`、`scripts/` 在一起。Claude Code 用 `/plotter`，Codex 用 `$plotter`。Skill 可独立于网站使用，不依赖本地跑官网（本地跑官网需要 Bun）。

## 注意事项

- **发帖人不是作者。** Viking（@vikingmute）是推荐者。项目 MIT，作者 Lucas Marques。
- **与 Linear 的关系。** 发帖人说自己喜欢「linear 的互动效果」。官网 Inspo 页确认感觉参考来自 linear.app 上三幅会响应指针的小线稿，并写明参考图属于 Linear、仅作参考；Hairline 的 figure 和代码是原创，与 Linear 没有隶属关系。
- **致敬标志不在包装里。** 随包装发布的是 33 个 figure。图鉴最后一架的 Vercel / Mastra / Notion 是用 skill 画的致敬稿，标志归其所有者，Hairline 声明未与这些公司关联。`hairline-adopt` 文档写明它不会描摹原 SVG，而是在同一套引擎上按实体重新搭建；若标志属于他人，skill 会告知。
- **依赖与环境。** 运行时零依赖，ESM only。React 18 及以上只是可选 peer，仅 `@lucasmarkes/hairline/react` 需要。开发该 monorepo 的根 `package.json` 写了 `engines.node >= 22`；已发布的 npm 包没有单独声明 engines。
- **无障碍。** figure 默认是带英文描述的 image，可用 `label` / `aria-label` 替换。Riffle 例外：可聚焦，方向键翻卡片，并由 live region 读出。`prefers-reduced-motion` 下，会自行播放的 Phosphor / Slow 以及设置了 `play` 的 figure 会停住，但文档写明它们仍会响应指针。
- **赞助是可选的。** 库本身 MIT 免费。GitHub Sponsors 用来资助后续 figure，并换取官网 / README 上的位置（Featured 250 美元/月起）。不赞助也能用。
- 2026-11-15 查看时 Stars 3,867、fork 239、7 个未关闭 issue。仓库在 2026-11-13 仍有推送，可能含尚未进入 0.5.1 的提交。帖子附 23 秒演示视频，本次没有逐帧观看，描述以帖子正文、官网和 README 为准。
- **Plotter 的发帖人不是作者。** sundyme 是推荐者。项目作者是 Pasquale Vitiello（@pacovitiello）。当前项目与可分发 skill 包均为 MIT。LICENSE 版权行同时写着 “Copyright (c) 2025 coss.com and Origin UI” 与 “Copyright (c) 2026 Pasquale Vitiello”。`ATTRIBUTION.md` 说明 Plotter 是从 coss 仓库抽出的独立项目；维护者在 2026-11-08 选定 MIT。抽取当时根目录曾带过 AGPL-3.0 记录。随 skill 打包的 Cal Sans 为 SIL Open Font License 1.1，不是 MIT。`package.json` 版本 0.1.0，无 engines 字段。画图仍要消耗已登录 Agent 的额度。
- **Plotter 与 Hairline 不是同一项目。** Hairline 是 33 个会响应指针的现成等距 line figure 库；Plotter 是生成新的构造线 SVG / HTML 动画的 Skill。
- 评论区有使用者说这种风格画架构图、数据流程图比画产品图更稳，以及 Claude 直接改 path 时可能生成冗余图层、导出前最好清理。这是评论者经验，作者未确认。发帖人只回了「感谢反馈」。原作者在自己的帖子里对 “Is this free to use?” 回了 “yesss”。演示视频 23 秒，本次未观看。官网图鉴页 2026-11-20 查看时可数到 109 个编号插画；文档没有另给一个官方总数。2026-11-20 查看时 Stars 194、fork 10、2 个未关闭 issue。
