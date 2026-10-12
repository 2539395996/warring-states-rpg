# AGENTS.md — Codex 本地执行边界

1. 本仓库为《战国立志传》项目。必须遵守公元前300—前221年历史可玩范围（79年，<=100）。
2. 读取 `README.md`、`00_context/01_PROJECT_LOCKS.md`、主控 MD，以及当前 `03_tasks/ready/*.json` 中单个已批准任务。
3. **禁止未经明确授权修改**旧《洪武》Unity 工程、旧 Godot 项目、太阁解包研究数据；只读审核可以。
4. 对未经用户批准的设计文件不能自作决定改游戏范围；架构关键冲突写到任务报告并请求 ADR。
5. 修改只在任务 `allowed_write_paths`，任何越界修改须停止、记录并请求授权。
6. 一任务一分支，先检查 `git status`、版本和工具，严禁删除已有在途变更、乱用 `git reset --hard`。
7. 测试结果必须有真实命令与退出码；`NOT_RUN` 不是 `PASS`；涉及 UI 和战斗要附截图/录屏及可操作路径。
8. 每个任务结束生成 `04_reports/TASK-xxx-REPORT.md`，列出改动、依赖、执行命令、失败及下一任务建议；不得自行标记 DONE。
9. 新 Godot 工程优先 Windows/Godot 4 .NET + 纯 C# simulation；禁止声称 C# Godot 4 工程直接可 Web 导出。
10. 视觉/音频资产必须原创或获授权；不提交原版太阁 DDS/反编译原脚本，也不提交密钥或凭据。
