# 史上最強動漫 - 咒術迴戰角色介紹 Hub (Jujutsu Kaisen Summer Portal)

這是一個以清爽天藍夏日風格設計的《咒術迴戰》角色圖鑑與術式資料庫網站。專案具備完整 RWD 響應式網頁設計、SEO 優化、動態搜尋與過濾、分頁模組及詳細的對話彈窗數值圖表。

## 📁 專案目錄結構 (Directory Structure)

本專案採用模組化 CSS 設計與獨立的圖片資料匣，非常適合部署至 GitHub Pages、Vercel 或 InfinityFree。

```text
jujutsu-kaisen-app/
├── index.html              # 核心 HTML 結構與 SEO 標籤、JS 邏輯
├── css/                    # 切割後的 CSS 檔案匣
│   ├── variables.css       # 天藍色系變數與主題調色
│   ├── reset.css           # CSS 重置設定
│   ├── layout.css          # Grid 系統、Sidebar & RWD
│   └── components.css      # 卡片、彈窗、分頁按鈕
├── images/                 # 角色圖片資料匣 (images/)
│   ├── gojo.jpg            # 五條悟
│   ├── nanami.jpg          # 七海建人
│   ├── choso.jpg           # 脹相
│   └── sukuna.jpg          # 兩面宿儺
├── prompt-guide.md         # AI Prompt 指令說明文件 (.md)
└── README.md               # GitHub 說明檔
