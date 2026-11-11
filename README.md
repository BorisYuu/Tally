# Tally 外殼頁面（放到 GitHub Pages）

這個資料夾讓 Tally 可以：用你的圖示、全螢幕像 App 一樣開啟、不顯示 Google 的通知列。

## 1. 填入網址
用文字編輯器打開 `index.html`，找到這一行：

    var APP_URL = 'https://script.google.com/macros/s/請貼上你的部署ID/exec';

換成你的 Apps Script 網頁應用程式網址（Apps Script →「部署 → 管理部署作業」可以複製，結尾是 `/exec`）。

## 2. 放上 GitHub Pages
1. GitHub → New repository → 名稱例如 `tally` → Public → Create
2. Add file → Upload files → 把這個資料夾裡的檔案**全部**拖進去（index.html、manifest.webmanifest、所有 png）→ Commit
3. Settings → Pages → Branch 選 `main`、資料夾 `/ (root)` → Save
4. 等 1–2 分鐘，網址會是 `https://你的帳號.github.io/tally/`

> repo 是公開的也沒關係：裡面沒有密碼，資料也不在這裡。密碼只存在你的 iPhone 和 Apps Script 裡。

## 3. 加到 iPhone 主畫面
1. 刪掉舊的 Tally 捷徑／主畫面圖示
2. 用 **Safari** 打開 `https://你的帳號.github.io/tally/`
3. 分享按鈕 →「加入主畫面」→ 名稱已經是 Tally → 加入
4. 從主畫面打開，第一次輸入 Tally 密碼（之後會記住）
