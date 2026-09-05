# 樂活Villa － 羽過天輕

宜蘭五結包棟民宿．一頁式官方網站。

**線上網址：** https://din0326.github.io/luohuo-villa/

## 檔案結構

- `index.html` — 整個網站（HTML／CSS／JS 全部在同一個檔案內，沒有相依套件）
- `images/` — 網頁用照片（已壓縮，長邊 1500px）
- `.nojekyll` — 讓 GitHub Pages 直接輸出檔案，不做 Jekyll 處理

## 怎麼修改內容

直接編輯 `index.html` 即可，房價、房型、聯絡方式都是純文字。改完後：

```
git add -A && git commit -m "更新房價" && git push
```

推上去大約 1 分鐘後網站就會更新。

## 之後要接自有網域

1. 在 repo 根目錄新增一個 `CNAME` 檔，內容寫網域（例如 `www.luohuovilla.com`）
2. 到網域商設定 DNS：`www` 指向 `din0326.github.io`（CNAME 記錄）
3. GitHub repo 的 Settings → Pages 勾選 Enforce HTTPS
4. 記得把 `index.html` 裡 `og:image` 的網址一併換成新網域
