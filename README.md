# 战国立志传：Claude 设计协作仓库（R2.0）

这是**策划/研究/程序交接用私人仓库模板**，不是已经制作好的游戏。最高需求见 [《战国立志传》完整重构项目总控方案](战国立志传_完整重构项目总控方案.md)。

- **可玩时间严格限定前300—前221年（跨度79年）**。重点首版为前265年开局。
- **Claude 网页聊天**仅负责设计、历史研究、系统契约、任务/报告审核；**本地 Codex**才修改 Godot、执行编译和测试。
- 优先 Godot 4 .NET / Windows 原型，具体版本由本地审计冻结。
- **旧《洪武立志传》汇总放 `01_research/legacy/`**，仅用于研究与可复用架构；旧 Unity 工程不上传、不覆盖。
- 上传清单见 [`00_context/00_START_HERE.md`](00_context/00_START_HERE.md)，GitHub/Claude 的连接与刷新见 [`00_context/02_GITHUB_HANDOFF.md`](00_context/02_GITHUB_HANDOFF.md)。

注意：**GitHub 私有仓库不等于 Claude 已自动读取**，必须在 Claude 聊天或 Projects 中选择相应文件，并在更新后同步。不要上传 API Key、非授权太阁原素材或整个旧 Unity 工程。
