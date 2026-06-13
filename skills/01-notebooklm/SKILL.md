---
name: codex-notebooklm
description: Codex 連接 NotebookLM MCP。說「連接 NotebookLM」時載入。
---

# 連接 NotebookLM（Codex 版）

1. 檢查 `uv --version`，再執行 `uv tool install notebooklm-mcp-cli`；已安裝則用 `uv tool upgrade notebooklm-mcp-cli`
2. 驗證 `nlm --version` 與 `Get-Command nlm, notebooklm-mcp`
3. `nlm login`，再用 `nlm login --check` 驗證
4. 註冊 MCP：`codex mcp add notebooklm -- notebooklm-mcp`
   或手動編輯 `~/.codex/config.toml`：
```toml
[mcp_servers.notebooklm]
command = "notebooklm-mcp"
startup_timeout_sec = 60.0
tool_timeout_sec = 120.0
```
5. 重啟 Codex 後驗證：列出筆記本
6. 建立一個明確標記為測試的 notebook，確認後立即刪除

注意：`nlm mcp` 已失效，不可再使用。這是非 Google 官方工具，使用內部 API；不要提交登入憑證。回報：nlm 版本、登入狀態、MCP 設定、建立/刪除測試結果。
