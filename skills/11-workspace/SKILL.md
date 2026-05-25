---
name: codex-workspace
description: Codex 專案初始化工作模式。說「初始化專案」「老師建專案」時載入。
---

# 專案初始化（Codex 版）

1. 問：名稱、用途、資料夾、GitHub repo、公開/私有、部署需求
2. 建立：AGENTS.md、README.md、.gitignore、Git repo、GitHub repo、Obsidian 工作筆記
3. 確認 Codex 全域 skills：`startup-sync`、`shutdown-sync`、`project-init-sync` 已在 `~/.codex/skills/`

## 開工/收工
開工：使用 `startup-sync`，讀 AGENTS.md → 讀 Obsidian 筆記 → git status → 回報
收工：使用 `shutdown-sync`，檢查敏感資料 → 更新筆記 → git commit/push → chezmoi 同步（見 13-chezmoi）

回報：檔案清單、GitHub URL、Obsidian 筆記路徑。
