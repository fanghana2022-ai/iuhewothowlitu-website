# 史上最強動漫 - 咒術迴戰角色介紹 Hub (Jujutsu Kaisen Character Hub)

![Jujutsu Kaisen Banner](https://nxsnjqfqtwiaoedulnpr.supabase.co/storage/v1/object/public/image/articles/33-1_13e74e51-97ec-48c6-9f1d-9b9c2a6b1ed2_f00d3cf41f4d.jpg)

An interactive, responsive, and beautifully designed web repository for **Jujutsu Kaisen** characters, techniques, and domain expansions. Built with a modern summer sky-blue color scheme, seamless search/filtering capabilities, dynamic pagination, and visual character stat breakdowns.

---

## 📖 目錄 (Table of Contents)

- [專案簡介](#-專案簡介)
- [核心功能特色](#-核心功能特色)
- [技術棧與開發工具](#-技術棧與開發工具)
- [專案目錄結構](#-專案目錄結構)
- [SEO 與 RWD 響應式架構](#-seo-與-rwd-響應式架構)
- [本地開發與運行](#-本地開發與運行)
- [平台部署指南](#-平台部署指南)
  - [InfinityFree 部署](#1-infinityfree-託管)
  - [GitHub Pages 部署](#2-github-pages-託管)
  - [Vercel 部署](#3-vercel-一鍵部署)
- [授權與版權聲明](#-授權與版權聲明)

---

## 🌟 專案簡介

本專案是一個專為《咒術迴戰》粉絲與動漫愛好者打造的角色資料庫網站。網頁採用清爽天藍夏日風格（Summer Sky Blue Theme），結合現代化的 **Glassmorphism（玻璃擬態）** UI 設計，提供流暢的互動體驗。

使用者可於網站中瀏覽包含五條悟、兩面宿儺、乙骨憂太、夏油傑、伏黑甚爾等熱門角色的詳細檔案、生來術式、領域展開介紹以及視覺化戰鬥能力進度條。

---

## ✨ 核心功能特色

1. **即時關鍵字搜尋 (Real-time Search)**
   - 支持角色中文姓名、羅馬拼音、術式名稱或領域展開名稱的即時比對過濾。

2. **多維度分類與篩選 (Category Filtering)**
   - 提供側邊欄陣營分類（高專學生、特級/一級術師、詛咒師/詛咒之王、受胎九相圖、天與咒縛/殺手）。
   - 側邊欄動態顯示各分類對應的角色數量統計。

3. **靈活的排序機制 (Sorting System)**
   - 支持按「預設排序」、「戰鬥力 (高至低)」、「角色姓名 (A-Z)」進行資料重整。

4. **動態分頁模組 (Dynamic Pagination)**
   - 前端 JavaScript 自訂分頁邏輯，動態計算頁碼、前頁/後頁切換與當前顯示筆數。

5. **互動式角色詳情彈窗 (Interactive Modal Showcase)**
   - 點擊角色卡片可開啟全螢幕視窗，展示高清角色立繪、所屬單位、完整背景介紹以及攻擊、防禦、速度與領域強度的長條視覺化圖表。

6. **開發架構預覽 Modal**
   - 內建專案架構與部署說明彈窗，便利開發者直接於前端檢視目錄與 deployment 說明。

---

## 🛠 技術棧與開發工具

- **前端核心**：HTML5, Pure JavaScript (ES6+)
- **CSS 框架與樣式**：
  - [Tailwind CSS CDN](https://tailwindcss.com/)（快速 RWD 與 utility-first 佈局）
  - Custom CSS3 Variables（主題天藍色調系統與 Glassmorphism 視覺特效）
- **圖示庫**：[FontAwesome 6.4.0](https://fontawesome.com/)
- **字型**：[Google Fonts - Noto Sans TC](https://fonts.google.com/specimen/Noto+Sans+TC)

---

## 📁 專案目錄結構

本專案支援將 CSS 與圖片資源獨立拆分，保持目錄簡潔且易於維護：

```text
jujutsu-kaisen-app/
├── index.html               # 核心 HTML 結構、SEO 標籤與 JS 控制邏輯
├── css/                     # 模組化 CSS 樣式檔案匣
│   ├── variables.css        # 天藍色系 CSS 變數與主題調色
│   ├── reset.css            # CSS Reset 設定
│   ├── layout.css           # Grid 系統、Sidebar & RWD 佈局
│   └── components.css       # 卡片、彈窗、分頁與 Badge 按鈕
├── images/                  # 角色圖片與 OG 社群分享圖庫
│   ├── og-jujutsu.jpg       # Open Graph 社群分享圖
│   ├── gojo.jpg             # 五條悟卡片圖
│   ├── nanami.jpg           # 七海建人卡片圖
│   ├── choso.jpg            # 脹相卡片圖
│   └── sukuna.jpg           # 兩面宿儺卡片圖
├── prompt-guide.md          # AI Prompt 指令說明文件 (.md)
└── README.md                # 專案說明文件 (.md)
```

---

## 📱 SEO 與 RWD 響應式架構

### 🔍 完整 SEO 優化
- **Meta 關鍵字與描述**：配置精準的動漫 SEO 標籤（`keywords`, `description`, `author`）。
- **Open Graph (OG) 協議**：支援 Facebook、LINE、Discord 等社群平台連結預覽卡片。
- **JSON-LD 結構化資料**：導入 Google Schema.org `WebPage` 結構化語法，提高搜尋引擎理解度。

### 📱 RWD 響應式適配
- **Desktop (≥ 1024px)**：採用 270px 雙欄佈局（Sidebar + Main Content Grid）。
- **Tablet / Mobile (< 1024px)**：自動轉為單欄流體佈局，側邊欄收合為抽屜式選單，可透過 Header 的漢堡按鈕（Hamburger Button）切換開關。

---

## 🚀 本地開發與運行

本專案為無編譯依賴的純靜態網頁（Vanilla HTML/JS），只需將檔案儲存至本地即可運行：

1. 克隆專案或下載 Zip 檔：
   ```bash
   git clone https://github.com/your-username/jujutsu-kaisen-app.git
   ```
2. 進入專案目錄：
   ```bash
   cd jujutsu-kaisen-app
   ```
3. 使用瀏覽器直接開啟 `index.html`，或使用 VS Code 的 **Live Server** 套件啟動本地開發伺服器。

---

## ☁️ 平台部署指南

### 1. InfinityFree 託管
1. 登入 InfinityFree 控制台，進入 **Control Panel (cPanel)**。
2. 打開 **Online File Manager** 並定位至 `htdocs/` 資料夾。
3. 將本專案的所有檔案與資料夾（`index.html`, `css/`, `images/`）完整上傳至 `htdocs/` 內。

### 2. GitHub Pages 託管
1. 將專案 Push 至 GitHub 儲存庫：
   ```bash
   git add .
   git commit -m "feat: initial commit for Jujutsu Kaisen Hub"
   git push origin main
   ```
2. 前往 GitHub Repository 頁面 $\rightarrow$ **Settings** $\rightarrow$ **Pages**。
3. 在 **Source** 選項選擇 `main` 分支與 `/root` 資料夾，點選 Save 即可發布網站。

### 3. Vercel 一鍵部署
1. 登入 [Vercel](https://vercel.com/) 並點選 **Add New Project**。
2. 連結 GitHub 帳號並選擇 `jujutsu-kaisen-app` 儲存庫。
3. 保持 Framework Preset 為 `Other` (Static HTML)，點擊 **Deploy** 即可完成自動 CI/CD 部署。

---

## 📜 授權與版權聲明

- **文字與程式碼**：採用 [MIT License](LICENSE) 授權開放使用。
- **動漫素材版權**：《咒術迴戰》（Jujutsu Kaisen）之角色名稱、美術圖鑑與設定版權均歸 **芥見下下（Gege Akutami） / 集英社（Shueisha） / MAPPA / 咒術迴戰製作委員會** 所有。本專案僅供個人學習與展示開發作品使用，無任何商業營利行為。

---

© 2026 Jujutsu Kaisen Summer Portal. Designed & Developed by **方榆涵**.
