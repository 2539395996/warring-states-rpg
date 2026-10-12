# 05 · Windows 将资料包上传为私有 GitHub 仓库

## 推荐 GitHub Desktop（无需写命令）
1. 解压本资料包，将 `WarringStates_Claude_Repo` 中**所有内容**放在一个本地目录，如 `D:\Projects\WarringStatesRPG`。
2. GitHub Desktop → File → Add local repository（如果还不是 Git 仓库，选择 Create a repository here）。
3. Commit 本地资料 → Publish repository → 勾选 **Keep this code private**。如先在 GitHub 新建仓库，避免同时初始化两套冲突的 README。
4. 在 github.com 检查根目录是否存在完整主控 MD 和 `00_context`、`01_research`。
5. 在 Claude Projects → Project knowledge `+ → GitHub`，完成私有仓库授权，先选少量关键文件，验证 Claude 可复述历史边界。

## 如用 Git 命令
建立 GitHub **空的 Private 仓库**，在本地解压目录运行：
```powershell
cd D:\Projects\WarringStatesRPG
git init
git branch -M main
git add .
git status
git commit -m "docs: initial warring states design brief"
git remote add origin https://github.com/<YOUR_USERNAME>/warring-states-rpg.git
git push -u origin main
```
`git add .` 的前提是**已先核实 `.gitignore`、仓库里不包含个人凭据/未经授权的原版太阁素材/旧游戏二进制**。`<YOUR_USERNAME>` 换成实际帐号。如果 Git 已初始化/已有 remote，按真实状态处理，不要强制重置。

**请注意**：本资料包只是文档、示例任务与研发规范，不包含完整 Godot 游戏工程。上传后只让 Claude 阅读选中内容，不自动替用户写代码。GitHub 网页浏览器上传通常单文件限 25 MiB；需要大素材时用 Git LFS，但此 MD 无需 LFS。
