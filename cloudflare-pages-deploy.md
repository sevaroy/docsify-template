# Cloudflare Pages 部署教學（適用 Docsify 專案）

本文件將指引你如何將本 Docsify 專案部署到 Cloudflare Pages，讓你的旅遊部落格能在網路上公開瀏覽。

---

## 一、前置需求

1. 已註冊 [Cloudflare 帳號](https://dash.cloudflare.com/sign-up)。
2. 專案已推送到 GitHub（或 GitLab）。

---

## 二、建立 Cloudflare Pages 專案

1. 登入 [Cloudflare Dashboard](https://dash.cloudflare.com/)。
2. 點選左側「Pages」>「Create a Project」。
3. 選擇你的 GitHub 帳號並授權 Cloudflare 存取你的 repo。
4. 選擇本 Docsify repo 並點選「Begin setup」。

---

## 三、部署設定

- **Production branch**：通常為 `main` 或 `master`。
- **Build command**：留空（Docsify 是純靜態網站，不需編譯）。
- **Build output directory**：填寫 `./` 或 `.`（根目錄）。

> 若出現「No build command」警告，請忽略。

---

## 四、完成部署

1. 點選「Save and Deploy」。
2. Cloudflare Pages 會自動建立並部署專案。
3. 部署完成後，你會獲得一組公開網址。

---

## 五、常見問題

### Q1. 為什麼網站顯示空白？
- 請確認 `index.html` 是否在專案根目錄。
- 請確認 output directory 設定為 `./`。

### Q2. 如何自訂網域？
- 進入 Cloudflare Pages 專案設定 > Custom domains，依指示綁定自有網域。

---

如有其他疑問，請參考 [Cloudflare Pages 官方文件](https://developers.cloudflare.com/pages/) 或提出 issue。
