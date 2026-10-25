# AI Agent 工具

以下仓库整理自丹丹爱学习（@dandanetha）2026-10-24 的帖子：<https://x.com/dandanetha/status/2113852735330365607>

Stars 和更新日期来自 GitHub API，查询于 2026-10-25（北京时间），更新日期按最后一次推送换算为北京时间；帖子里写的「66.5k Star」低于现值。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 给 AI Agent 接上它自己够不着的互联网：一个 CLI 搜索 / 读取 B站（含字幕）、小红书、X、Reddit、YouTube、GitHub、雪球、LinkedIn、网页等，每个平台失败自动换备选工具 | Python | 101,828 | 2026-10-23 | MIT | 让 Claude Code / Codex / Cursor 等 Agent 查中文平台、拿视频字幕、读登录墙后的内容（只读） | [@dandanetha 2026-10-24](https://x.com/dandanetha/status/2113852735330365607) | 2026-10-25（北京时间） |

安装方式：把这句发给 Agent：

    帮我安装 Agent Reach：https://raw.githubusercontent.com/Panniantong/Agent-Reach/main/docs/install.md

## 注意事项

- 需要登录的平台（小红书、X、Reddit 等）会把你 Chrome 里该网站的登录复制到它自己的专用浏览器，通常是主账号；平台可能限制自动访问的账号，README 建议换成小号。
- X、Facebook、Instagram 渠道标为「实验」，平台反爬更严，可能随时失效；YouTube 语音转文字、小宇宙播客转文字需要 Groq 或 OpenAI Key。
- 只从 GitHub 的 install.md 安装；PyPI 上叫 `agent-reach` 的包不是本项目。项目没有任何代币或加密项目。
- 帖子说「API 费用为零」：README 的说法是各渠道尽量免费，但语音转文字需要自备 Key。
