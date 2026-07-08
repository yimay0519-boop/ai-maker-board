# 🤖 AI 創客共學群討論版 (AI Maker Study Group Board)

這是一個專為 AI 創客共學群打造的**輕量化、全互動式討論版網站**。整合了「會議資訊公告」與「社群互動問答機制」，能完美協助團隊或班級進行知識萃取與技術交流。

## 🌟 核心特色
- **零後端部署成本**：採用前端架構與瀏覽器內建的 `LocalStorage` 技術，**不需額外搭建資料庫或伺服器**，直接點擊即可在任一網頁或移動端運行！
- **極速載入與精美 UI**：基於最新版 Tailwind CSS 構建，支援 RWD 自適應排版（手機、平板、電腦皆能優雅操作）。
- **一鍵部署 GitHub Pages**：檔案結構極簡安全，非常適合發佈至 GitHub 免費靜態網站代管空間。

---

## 🛠️ GitHub Pages 快速部署指南

只需 **4 個步驟**，即可將這個討論版網站發佈上線並分享給所有同學：

### 1. 建立一個新的 GitHub 儲存庫 (Repository)
- 登入您的 GitHub 帳號。
- 點擊右上角的 `+` 號 -> 選擇 **New repository**。
- 填寫儲存庫名稱（例如：`ai-maker-board`）。
- 將權限設為 **Public (公開)**（*注意：GitHub 免費版帳號必須是公開庫才能開啟 Pages 網站功能*）。
- 點擊下方 **Create repository** 建立。

### 2. 上傳網頁原始碼檔案
- 在您的電腦中，確保本專案包含以下兩個核心檔案：
  - `index.html` (主網頁程式碼)
  - `README.md` (說明文件)
- 在 GitHub 網頁畫面上點擊 **uploading an existing file** 連結。
- 將 `index.html` 和 `README.md` 拖曳上傳至網頁中。
- 在下方的 Commit 訊息欄位輸入 `Initial commit`，然後點擊 **Commit changes** 儲存。

### 3. 開啟 GitHub Pages 網頁功能
- 進入該儲存庫的 **Settings (設定)** 頁籤（上方齒輪圖示）。
- 在左側選單中，找到 **Code and automation** 區塊，點擊 **Pages**。
- 在 **Build and deployment** 下方的 **Source** 選擇 `Deploy from a branch`。
- 在 **Branch** 的下拉選單中，將原本的 `None` 改選為 `main` (或 `master`) 分支，右側資料夾保持 `/ (root)`。
- 點擊 **Save** 按鈕。

### 4. 取得您的專屬專案網址
- 點擊儲存後，大約等待 1 到 2 分鐘，重新整理該 Pages 設定頁面。
- 頂端將會出現一行綠色背景的提示訊息，顯示：**"Your site is live at..."** - 後方即是您的專屬專案網站連結！網址格式通常為：
  `https://<您的GitHub帳號>.github.io/ai-maker-board/`
- 將這個網址複製並發佈到班級群組，所有同學就能同步登入、查看會議資訊並進行問答互動了！

---

## 💡 使用小叮嚀與進階擴充
1. **資料儲存機制**：此版本資料完全儲存在使用者的「個別瀏覽器本地快取 (LocalStorage)」中。
2. **適合情境**：適合個人紀錄、小組內各自記錄學習日誌，或作為展示、作業成品提交。
3. **多人共用即時同步（若未來需擴充）**：如果您需要達成「A 同學發問，B 同學在自己電腦上能**立刻看見並回覆**」的全局即時同步功能，未來僅需將本程式中的 `localStorage` 讀寫邏輯，改為串接免費的雲端資料庫（如 Firebase Realtime Database 或 Supabase API），前端 HTML 介面完全不需重寫即可無縫升級！
