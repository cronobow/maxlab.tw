# MaxLab

個人作品與網頁開發服務的一頁式靜態網站，使用原生 HTML / CSS，無後台、資料庫或第三方前端依賴。

主要網域：https://maxlab.tw/ ；www.maxlab.tw 應導向主要網域。

## 本機預覽

```sh
python3 -m http.server 8080 --bind 127.0.0.1
```

開啟 http://127.0.0.1:8080 。

- `index.html`：內容與連結。
- `assets/style.css`：版型與本機 CSS 插畫。
- `assets/favicon.svg`：網站圖示。
- `.github/workflows/pages.yml`：手動發布至 GitHub Pages。

## 發布

Repository 的 Settings → Pages 使用 GitHub Actions，Custom domain 設為 `maxlab.tw`。修改後先預覽並驗證，再推送 main，手動執行 Deploy static site to GitHub Pages。確認 workflow 對應發布版本、正式頁面及 HTTPS 正常。

發布檔案僅包含 index.html、assets、CNAME 與 .nojekyll。README 與開發檔案不打包至網站。

## 內容與隱私

- 明湖午餐資訊站與鮮乳條碼工具為公開作品，提供外連。
- 其餘六個作品同等展示、不附網址；所有插畫均為重新繪製，沒有真實使用者資料。
- 聯絡方式為 hello@maxlab.tw，使用 mailto，不含寄信表單。
- 不使用追蹤碼、Cookie、瀏覽器儲存、外部字型或嵌入服務；託管服務可能處理連線紀錄。
- 不提交金鑰、個人資料、帳務、群組對話、兒童照片、私人網址、客戶資料或舊站備份。
- 更新內容時維持上述公開範圍；正式發布須有明確授權。

## 網域與舊網站

DNS 與 GitHub Pages 自訂網域設定必須一致，www 指向 cronobow.github.io。維護網站 DNS 不應變更郵件 MX / TXT 記錄。舊 WordPress 文章未遷移；保留舊主機，另行決定封存與轉址方式。

GitHub 官方設定文件：https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
