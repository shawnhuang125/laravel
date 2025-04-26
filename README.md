# Laravel應用開發

## 環境安裝
- [說明文件]()
###  Laravel 完整專案架構說明 (開發文件)

#### 資料夾與目錄用途

| 資料夾或檔案 | 用途 | 應該放的內容 |
|--------------|------|----------------|
| `app/` | 核心應用程式目錄 | 控制器、模型、服務層邏輯 |
| ├— `Http/Controllers/` | 控制器 | 每個頁面或 API 的控制邏輯 |
| ├— `Models/` | Eloquent 資料模型 | 每個資料表對應的 PHP 類別 |
| ├— `Http/Middleware/` | 中介層 | 處理請求前/後的邏輯 |
| `bootstrap/` | 啟動應用程式核心 | Laravel 啟動設定，不需修改 |
| `config/` | 各類設定檔 | `app.php`、`database.php` 等設定 |
| `database/` | 資料庫相關 | `migrations`、`seeders`、`factories` |
| ├— `migrations/` | 資料表結構 | 定義資料表欄位與建立方式 |
| ├— `seeders/` | 初始資料填入 | 建立測試資料、預設帳號 |
| `public/` | 公開入口與資源 | `index.php` 入口檔、圖片、CSS、JS |
| `resources/` | 前端資源（Blade、Vue、CSS） | 前端視圖與樣式 |
| ├— `views/` | Blade 模板 | 後端演算頁面，像是 `welcome.blade.php` |
| ├— `js/` | Vue、JS | 前端組件、Vue 路由、axios 請求 |
| ├— `css/` | CSS 或 SCSS 檔案 | Tailwind、Bootstrap 或自訂樣式 |
| `routes/` | 所有路由定義 | `web.php`（給瀏覽器）、`api.php`（給前端 AJAX） |
| `storage/` | 快取、日誌、檔案上傳 | Laravel 自動使用的資料 |
| `tests/` | 測試程式碼 | 單元測試、功能測試 |
| `vendor/` | Laravel 套件 | Composer 安裝，自動產生，不要修改 |

---

#### 常見檔案說明

| 檔案 | 功能 |
|------|------|
| `.env` | 環境變數（資料庫連線、APP_KEY、API 金鑰） |
| `artisan` | Laravel CLI 指令列工具 |
| `composer.json` | PHP 套件管理器設定 |
| `package.json` | JavaScript 套件設定（如果有用 Vue/Vite） |
| `vite.config.js` / `webpack.mix.js` | 前端打包器設定檔（Laravel 10使用 Vite） |

---

#### 實作建議

- **API 請求寫在 `routes/api.php`**
- **前端樣式寫在 `resources/css/`，Vue 寫在 `resources/js/Pages/`**
- **Controller 放在 `app/Http/Controllers/`，Database 用 `migrations` 建立**
- **資料表用 `php artisan make:model Order -m` 同時建立 Model 與 Migration**

---

要不要我給你一個可以直接 clone 下來開發的空模板？（含前端+API執行）❤️



http://127.0.0.1:8000/
```




