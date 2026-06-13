---
name: codex-env-setup
description: Codex 環境建置（Codex Desktop、Node.js LTS、uv；CLI 選用）。說「建置環境」「安裝開發環境」時載入。
---

# Codex 環境建置

先確認作業系統與 Codex Desktop app 是否已安裝、登入。檢查：`node --version; uv --version`；只有使用者要用 CLI 時才檢查 `codex --version`。

| 工具 | Windows | macOS | Linux |
|------|---------|-------|-------|
| Node.js LTS | `winget install --id OpenJS.NodeJS.LTS --exact` | `brew install node` | 依 NodeSource LTS 指示安裝 |
| Codex CLI（選用） | 依 OpenAI Codex CLI 官方安裝頁 | 同左 | 同左 |
| uv | powershell iex script | `curl -LsSf ... \| sh` | 同左 |

使用 PowerShell 語法處理 Windows。不要因為缺少選用的 Codex CLI 就判定 Desktop 環境失敗。最終回報：已安裝/已補裝清單、版本、Codex 登入狀態。
