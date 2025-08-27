# 基弧選擇器（折射率 + 度數 → 基弧）

從折射率與度數快速查出建議基弧。資料來自您的 Excel 表格並已整理為靜態網站。

## 一鍵發佈到 GitHub Pages（最簡單）

1. 在 GitHub 建立一個 **public** repository，例如：`basecurve-picker`。
2. 上傳本資料夾內所有檔案（或直接 `git push`，見下方指令）。
3. 在 GitHub 專案頁面 → **Settings** → **Pages**：
   - **Source** 選擇 **GitHub Actions**（建議）。
   - 第一次 push 後，Actions 會自動跑佈署；完成後會看到你的網站網址。

> 也可選擇 **Deploy from a branch**，將 `main` 分支的根目錄（root）作為 Pages 來源。

## Git 指令（已安裝 git 的用戶）

```bash
# 將以下指令貼上終端機即可（請把 <YOUR_REPO_URL> 換成你的 GitHub 倉庫位址）
git init
git add .
git commit -m "Initial commit: basecurve picker"
git branch -M main
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```

## 本地預覽
直接雙擊 `index.html` 用瀏覽器開啟，或
```bash
# 任選一個簡易伺服器
python3 -m http.server 5500
# 開啟 http://localhost:5500
```

## 內容說明
- `index.html`：單一檔案應用（已內嵌資料表）。
- `basecurve_mapping.json`：對應表 JSON（可選，用於未來擴充）。
- `.github/workflows/pages.yml`：GitHub Actions 佈署流程。

## 授權
MIT