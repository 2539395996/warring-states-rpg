# 00 · 仓库读取入口

## Claude 首次阅读顺序
1. `README.md`（仓库性质与状态）
2. `00_context/01_PROJECT_LOCKS.md`（锁定需求）
3. `战国立志传_完整重构项目总控方案.md`（完整全案）
4. `00_context/04_DELIVERY_CONTRACT.md`（输出内容与审查）
5. `01_research/history/EVIDENCE_LEDGER.md`（历史证据规则）
6. `00_context/02_GITHUB_HANDOFF.md`（文件是否能读到及同步）
7. `00_context/03_CLAUDE_FIRST_MESSAGE.md`（本次工作命令）
8. `01_research/legacy/洪武立志传_整体提示词与太阁研究汇总_2026-10-12.md`（第一次架构复用审计时选读）

如果本清单某条不存在/未添加到 Claude 的 GitHub 选定范围，必须明确回答“未读取”，不能依据文件名伪称已看到。即使本地存在 `E:\` 路径，也不代表网页 Claude 可读。

## 权限边界
- **本文件和主控规范**优先于旧元末计划。
- `LOCKED` 不能擅改，`PROPOSED` 需论证，`RESEARCH` 需核证，`OPTIONAL` 需用户确认。
- 新 `02_design` 产物只有审核后成为 APPROVED；旧代码测试不等于新项目代码已通过。
- GitHub 集成通常读取选择分支上文件名/内容；不要假设能读取提交史、PR 或尚未 push 的本地文件。
