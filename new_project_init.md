# 專案初始化
- 專案`npm`套件安裝
```
npm install vue@3 @vue/compiler-sfc
npm install @inertiajs/inertia @inertiajs/inertia-vue3
composer require inertiajs/inertia-laravel
```
- 運行laravel專案(需開兩個終端介面分別運行)
- 在開發模式下編譯資源
```
npm run dev
```
- 連線至SQL Server
- 請執行以下 SQL 後再回 Laravel 測試連線功能
```
CREATE USER 'phpmyadmin'@'192.168.0.30' IDENTIFIED BY 'P@ssw0rd123!';
GRANT ALL PRIVILEGES ON laravel_database.* TO 'phpmyadmin'@'192.168.0.30';
FLUSH PRIVILEGES;
```
- 然後回到 Laravel 專案執行
```
php artisan config:clear
php artisan serve
```
### 專案解壓縮後的初始化
- 建議確認是不是解壓縮後多包了一層資料夾,如果有的化,只保留一層就正常了
- 解壓後要執行以下指令來重建 vendor：
```
composer install
```
### Policy更改
- ![image](https://github.com/user-attachments/assets/f75e43a1-9e54-41f0-ad71-34e27c02f237)
```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

- 按下鍵盤 Y。
- 按下 Enter。
- ![image](https://github.com/user-attachments/assets/dec32056-9c6e-4bb4-87a5-6bff4d8a9924)
