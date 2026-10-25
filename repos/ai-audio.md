# AI 音频

earshot 是用户自行补充的，不在 Levi 卧云（@zmdsb259414）2026-10-22 的帖子清单里：<https://x.com/zmdsb259414/status/2113140946699460933>

timeline-bgm 整理自风清扬（@hassanyehiaa）2026-10-22 的帖子：<https://x.com/hassanyehiaa/status/2113246930507899163>

可以和 [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft)、[lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) 搭配，给代码生成的影片配上音效。

Stars 和更新日期来自 GitHub API，查询于 2026-10-23（北京时间），更新日期按最后一次推送换算为北京时间。

| 仓库 | 用途 | 语言 | Stars | 最近更新 | 许可证 | 适用场景 | 来源 | 统计核对 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Leonxlnx/earshot](https://github.com/Leonxlnx/earshot) | 给编程 Agent 装上“耳朵”：让 AI 能听懂、评审并用代码生成声音，纯 CPU 本地运行，提供 CLI、Python API 和 MCP 服务 | Python | 2,198 | 2026-10-23 | MIT | 给代码做的视频配音效、检查音画同步、对照专业发布片打分 | 用户自行补充 | 2026-10-23（北京时间） |
| [xiaoyang111222/timeline-bgm](https://github.com/xiaoyang111222/timeline-bgm) | 免费、本地合成视频 BGM：按手写时间轴、分镜表或从 Remotion / HTML 工程提取的时间轴，按场景和关键时刻配乐 | Python | 15 | 2026-10-11 | 未声明 | 给 Remotion / Canvas 代码视频、短视频配背景音乐，不用付费音乐服务 | [@hassanyehiaa 2026-10-22](https://x.com/hassanyehiaa/status/2113246930507899163) | 2026-10-23（北京时间） |

## 注意事项

earshot 本体本地离线运行；可选的 `llm` 命令会把音频上传到 Gemini，需要自备 key 并显式同意。每次 CLI 调用都要重新加载模型（约 20–40 秒），调用多时建议用 MCP 服务或 Python API。

timeline-bgm 仓库没有 LICENSE 文件，README 也没写许可，按默认规则保留所有权利，复用代码前最好先问作者。它是程序化合成音乐，不是音乐生成模型，需要 Python（numpy、soundfile）和 ffmpeg。
