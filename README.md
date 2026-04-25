# My Notes Site

Personal reading log built with [Quarto](https://quarto.org/).

## Setup

```bash
# 1. Install Quarto
# https://quarto.org/docs/get-started/

# 2. Preview locally
quarto preview

# 3. Build
quarto render

# 4. Deploy to GitHub Pages (one-time setup)
quarto publish gh-pages
```

## Writing a new note

建立新檔案在 `posts/` 資料夾：

```
posts/YYYY-MM-DD-slug.qmd
```

YAML front matter 範本：

```yaml
---
title: "標題"
date: YYYY-MM-DD
categories: [ML, Paper]   # ML / Paper / Social Science / Philosophy / Tech
description: "一句話摘要，會出現在列表頁"
---
```

## Categories

- `ML` — 機器學習相關
- `Paper` — 學術論文
- `Social Science` — 社科、政策
- `Philosophy` — 哲學、人文
- `Tech` — 其他技術書籍

## File structure

```
my-site/
├── _quarto.yml       # 網站設定
├── index.qmd         # 首頁（Notes 列表）
├── about.qmd         # About
├── projects.qmd      # Projects
├── custom.scss       # 樣式調整
└── posts/            # 閱讀筆記放這裡
    ├── 2025-04-18-shap-practitioners.qmd
    └── 2025-04-09-housing-policy.qmd
```
