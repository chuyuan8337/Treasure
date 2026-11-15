# 交互线稿插画

以下仓库整理自 Viking（@vikingmute）2026-11-14 的帖子：<https://x.com/vikingmute/status/2121607129547043219>

发帖人不是项目作者。项目作者是 Lucas Marques（GitHub [lucasmarkes](https://github.com/lucasmarkes)，X [@lucasmarkes__](https://x.com/lucasmarkes__)）。

Stars 和更新日期来自 GitHub API，查询于 2026-11-15（北京时间），更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [lucasmarkes/hairline](https://github.com/lucasmarkes/hairline) | 33 个等距线稿 SVG 插画（figure），鼠标靠近会跟手反应，可用 intensity（0 到 1）调节强度；零依赖，支持 React 或纯 DOM，也可走 shadcn 注册表；另有 `/hairline-create` 和 `/hairline-adopt` 两个可选 Agent Skill，用来自画或从已有 SVG 生成 | TypeScript | 3,867 | 2026-11-14 | MIT | 给产品页、空状态或小彩蛋加有手感的线稿插画；或让 Agent 按同一套规则画出自己的 figure | [@vikingmute 2026-11-14](https://x.com/vikingmute/status/2121607129547043219) | 2026-11-15（北京时间） |

- 官网 / 图鉴：<https://hairline.lucasmarkes.com> 、<https://hairline.lucasmarkes.com/figures>
- 安装（摘自 README / 文档）：`npm i @lucasmarkes/hairline`；或 `npx shadcn@latest add https://hairline.lucasmarkes.com/r/hairline.json`
- Skill：`npx skills add lucasmarkes/hairline`，然后 `/hairline-create <idea>` 或 `/hairline-adopt <file.svg>`
- 当前发版：npm / CHANGELOG / 官网均为 0.5.1（2026-10-14）。文档写全套 33 个 figure 合计约 63.5 kB gzipped，只导入一个则只带上那一个。
- 33 个 figure 按主题分 8 架（与官网图鉴一致，已按 README 表核对）：Interfaces 1、Data 3、Machines 3、Devices 3、Coding 6、Security 3、Connectivity 6、Empty 8。

## 注意事项

- **发帖人不是作者。** Viking（@vikingmute）是推荐者。项目 MIT，作者 Lucas Marques。
- **与 Linear 的关系。** 发帖人说自己喜欢「linear 的互动效果」。官网 Inspo 页确认感觉参考来自 linear.app 上三幅会响应指针的小线稿，并写明参考图属于 Linear、仅作参考；Hairline 的 figure 和代码是原创，与 Linear 没有隶属关系。
- **致敬标志不在包装里。** 随包装发布的是 33 个 figure。图鉴最后一架的 Vercel / Mastra / Notion 是用 skill 画的致敬稿，标志归其所有者，Hairline 声明未与这些公司关联。`hairline-adopt` 文档写明它不会描摹原 SVG，而是在同一套引擎上按实体重新搭建；若标志属于他人，skill 会告知。
- **依赖与环境。** 运行时零依赖，ESM only。React 18 及以上只是可选 peer，仅 `@lucasmarkes/hairline/react` 需要。开发该 monorepo 的根 `package.json` 写了 `engines.node >= 22`；已发布的 npm 包没有单独声明 engines。
- **无障碍。** figure 默认是带英文描述的 image，可用 `label` / `aria-label` 替换。Riffle 例外：可聚焦，方向键翻卡片，并由 live region 读出。`prefers-reduced-motion` 下，会自行播放的 Phosphor / Slow 以及设置了 `play` 的 figure 会停住，但文档写明它们仍会响应指针。
- **赞助是可选的。** 库本身 MIT 免费。GitHub Sponsors 用来资助后续 figure，并换取官网 / README 上的位置（Featured 250 美元/月起）。不赞助也能用。
- 2026-11-15 查看时 Stars 3,867、fork 239、7 个未关闭 issue。仓库在 2026-11-13 仍有推送，可能含尚未进入 0.5.1 的提交。帖子附 23 秒演示视频，本次没有逐帧观看，描述以帖子正文、官网和 README 为准。
