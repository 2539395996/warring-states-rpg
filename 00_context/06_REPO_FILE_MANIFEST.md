# 06 · GitHub 上传文件分层索引

## 上传后第一轮让 Claude 读取（9个）
1. `README.md`
2. `00_context/00_START_HERE.md`
3. `00_context/01_PROJECT_LOCKS.md`
4. `00_context/02_GITHUB_HANDOFF.md`
5. `00_context/03_CLAUDE_FIRST_MESSAGE.md`
6. `00_context/04_DELIVERY_CONTRACT.md`
7. `战国立志传_完整重构项目总控方案.md`
8. `01_research/history/EVIDENCE_LEDGER.md`
9. `01_research/legacy/洪武立志传_整体提示词与太阁研究汇总_2026-10-12.md`（内容较长，可第二轮选读）

## 只需放仓库、不必一开始给 Claude 的
- `AGENTS.md`：Codex 约束（Claude 做任务审查时再添加）。
- `.gitignore`：避免提交凭据、缓存和未授权文件。
- `00_context/05_GIT_PUBLISH_WINDOWS.md`：给用户的操作说明。
- `03_tasks/ready/TASK-P0-001.json`：技术审计准备之后再让 Claude 看。
- `04_reports/README.md`：报告规范；真正报告由本地 Codex 后续产生。
- `05_tools/README.md` 与 `game/README.md`：目录预留，未实际开发。

## 完全不要上传到此设计仓库
旧 Unity/Godot 完整工程、原版太阁解包、大型构建产物、个人凭据、未授权图文/音乐。需要源代码审查时，让 Codex 写精简模块清单和测试证据；必要时仅将授权的 C# 源码文件另建私有代码仓库供 Claude 定向选择。
