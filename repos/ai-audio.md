# AI 音频

earshot 是用户自行补充的，不在 Levi 卧云（@zmdsb259414）2026-10-22 的帖子清单里：<https://x.com/zmdsb259414/status/2113140946699460933>

可以和 [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft)、[lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) 搭配，给代码生成的影片配上音效。

Stars 和更新日期来自 GitHub API，查询于 2026-10-23（北京时间），更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Leonxlnx/earshot](https://github.com/Leonxlnx/earshot) | 给编程 Agent 装上“耳朵”：让 AI 能听懂、评审并用代码生成声音，纯 CPU 本地运行，提供 CLI、Python API 和 MCP 服务 | Python | 2,198 | 2026-10-23 | MIT | 给代码做的视频配音效、检查音画同步、对照专业发布片打分 | 用户自行补充 | 2026-10-23（北京时间） |

## 注意事项

earshot 本体本地离线运行；可选的 `llm` 命令会把音频上传到 Gemini，需要自备 key 并显式同意。每次 CLI 调用都要重新加载模型（约 20–40 秒），调用多时建议用 MCP 服务或 Python API。
