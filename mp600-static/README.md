# MP600 Product Page - Static Version

## 檔案說明
這是 MP600 產品宣傳網頁的純靜態版本，可直接部署至任何靜態主機。

## 部署方式

### 方法一：本地預覽
1. 解壓縮 ZIP 檔案
2. 使用任何 HTTP 伺服器開啟（不能直接用檔案瀏覽器開啟 index.html）
   ```bash
   # 使用 Python
   python3 -m http.server 8000
   
   # 或使用 Node.js
   npx serve .
   ```
3. 在瀏覽器開啟 http://localhost:8000

### 方法二：部署至靜態主機
可部署至以下任一平台：
- **Netlify**: 拖曳整個資料夾至 netlify.com
- **Vercel**: 使用 Vercel CLI 或網頁介面上傳
- **GitHub Pages**: 推送至 GitHub 並啟用 Pages
- **AWS S3**: 上傳至 S3 bucket 並啟用靜態網站託管

## 注意事項
⚠️ 此為純靜態版本，以下功能已移除：
- 會員登入系統
- 文件下載權限控管
- 聯絡表單後端處理

所有文件（PDF）可直接公開下載，無需登入。

## 檔案結構
```
mp600-static/
├── index.html          # 主頁面
├── assets/             # CSS 與 JS 檔案
├── docs/               # PDF 技術文件
├── *.png               # 產品圖片
├── *.mp4               # 應用場景影片
└── README.md           # 本說明文件
```

## 技術規格
- 框架：React 19 + Vite
- 樣式：Tailwind CSS 4
- 字體：Roboto + Rajdhani (Google Fonts)
- 設計風格：Precision Engineering (精密工程美學)
