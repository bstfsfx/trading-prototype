# 股票分析平台 - 原型 (Vercel 部署)

## 部署狀態

| 項目 | 狀態 |
|------|------|
| 框架 | Vanilla HTML/CSS/JS |
| 部署平台 | Vercel |
| 語言 | 繁體中文 |

---

## 部署步驟

### 1. 推送至 GitHub

```bash
cd /Users/jackychau/Documents/GitHub/Sites/trading/prototype
git init
git add .
git commit -m "Initial prototype commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/trading-prototype.git
git push -u origin main
```

### 2. 連接到 Vercel

1. 前往 [vercel.com](https://vercel.com)
2. 點擊 "New Project"
3. 選擇 "Import Git Repository"
4. 選擇 `trading-prototype` repo
5. Vercel 會自動檢測為 Static Site
6. 點擊 "Deploy"

### 3. 自定義網域 (可選)

在 Vercel 項目設定中可以自定義網域。

---

## 專案結構

```
prototype/
├── index.html      # 主頁面 (繁體中文)
├── vercel.json     # Vercel 配置文件
└── README.md       # 本文件
```

---

## 功能預覽

- [x] 繁體中文介面
- [x] 響應式設計
- [x] 市場選擇 (香港/台灣/美國)
- [x] 快速股票按鈕
- [ ] 實際股票數據 (待連接 API)
- [ ] 互動式圖表 (待整合)

---

## 後續開發

原型完成後，可以：

1. **添加 API 端點** - 連接股票數據 API
2. **整合圖表庫** - 使用 Plotly 或 Chart.js
3. **添加后端** - 如果需要 Python 後端，遷移到 Railway/Render

---

## 注意事項

這是純前端原型，部署在 Vercel Edge Network 上，適合展示和 MVP。

如需完整功能 (真實股票數據、回測、預測)，需要部署完整 Flask 後端。