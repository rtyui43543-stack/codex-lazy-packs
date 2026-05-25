---
name: codex-draw
description: Codex 生圖指引（內建 Image Gen Skill + 進階 API）。說「生圖」「畫圖」時載入。
---

# 生圖（Codex 版）

## 路線 A：內建 Image Gen Skill（新手推薦）
直接用自然語言產圖，不需 API Key：
```
生成一張 16:9 的國中數學簡報封面圖，風格專業明亮，不要文字。
```
圖片存在：`~/.codex/generated_images/`

## 路線 B：API 路線（進階）
需要 `OPENAI_API_KEY` 時，先參考本 repo 的 `08-用Image Gen Skill在Codex生圖.md` 路線 B；不要直接套用 OpenCode 的 `~/.config/opencode/skills/` 路徑。

## 提示格式
```
用用途：...
尺寸比例：...
主題：...
風格：...
色彩：...
限制：...
```

⚠️ 重要中文文字建議後製；API Key 不寫進 repo。
