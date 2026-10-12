# 02 · GitHub / Claude 网页读取操作

**官方可核验文档**：https://support.claude.com/zh-CN/articles/10167454-使用-github-集成 （2026-09-02 更新）。

## GitHub 里先放什么
必须上传：`README.md`、`AGENTS.md`、`.gitignore`、`战国立志传_完整重构项目总控方案.md`、`00_context/00_START_HERE.md`、`00_context/01_PROJECT_LOCKS.md`、`00_context/02_GITHUB_HANDOFF.md`、`00_context/03_CLAUDE_FIRST_MESSAGE.md`、`00_context/04_DELIVERY_CONTRACT.md`、`01_research/history/EVIDENCE_LEDGER.md`。额外推荐上传 `01_research/legacy/洪武立志传_整体提示词与太阁研究汇总_2026-10-12.md`，**仅供审查旧机制与代码复用方案**。

先不用上传：整个 Unity 工程、旧 Codex 工作区、旧 Godot 大目录、原版太阁素材/解包、未授权史料 PDF、数 GB 音频、动画母版、`.godot/`、`bin/obj`、大日志和全部旧测试构建产物。等设计文件生成后再将批准的 `02_design/`、`03_tasks/` 和精简 `04_reports/` 逐步提交。

## Claude 普通聊天
聊天界面 `+ → 从 GitHub 添加` → 选仓库和上述关键文件，或 Claude Projects 的知识区 `+ → GitHub` → 选文件夹；私有仓库需授权对应 GitHub 仓库。文件更新后要在 Claude Projects 手动“同步”，或者在聊天中重新附加更新文件。与 Claude 核对选中的仓库、文件、分支、版本，别假定自动可读。

## 没有 GitHub 入口
改为上传主控 `.md` + `01_PROJECT_LOCKS.md` +旧研究汇总到 Claude 聊天；其余随阶段提交。给私有仓库 URL 不等于拥有阅读授权，也不等于 Claude 已读文件。

## 用户/GitHub Desktop
请阅读 `00_context/05_GIT_PUBLISH_WINDOWS.md`。仓库建议 Private；Claude GitHub 集成文件选择不应包含所有二进制与全部源码。

## 同步协议
1. Codex 完成工作、真实报告位于 `04_reports`；
2. 本地提交并 push；
3. 确认 GitHub 文件已更新；
4. Claude 手动刷新/重选文件，核对 Task ID 和 commit；
5. Claude 只给出审核结论或新任务，不能声称直接修改本地。
