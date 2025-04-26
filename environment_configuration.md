### 1. 安裝PHP
- 官方下載連結[下載連結](https://windows.php.net/download)
- ![image](https://github.com/user-attachments/assets/5e8b022d-2274-4384-b86e-34a4797884ce)
- 解壓縮
- ![image](https://github.com/user-attachments/assets/0e142a67-8d7e-4c08-a60c-46a8c05cd8dd)
- 複製`php.ini-development` 複製一份並重新命名為 `php.ini`
- ![image](https://github.com/user-attachments/assets/ae9d8293-589a-48d3-8c46-197ba1fcee24)
- ![image](https://github.com/user-attachments/assets/fcedc0f8-f8dd-4064-a66d-53ecb6117e88)

- 使用VScode/notepad編輯`php.ini`
- 將以下內容貼到該檔案的最底部
- ![image](https://github.com/user-attachments/assets/5a014381-55e1-407f-a6d0-524400a3edb0)
- 把 PHP 安裝路徑加到環境變數 Path 裡面
```
C:\php\php-8.4.6-Win32-vs17-x64\
```
- ![image](https://github.com/user-attachments/assets/1b3588d4-869e-466d-bab3-6ab5120660e9)
- ![image](https://github.com/user-attachments/assets/61e29d94-d8fb-4536-a369-90949be4e16a)
- ![image](https://github.com/user-attachments/assets/5acc8b41-9ffc-43f8-88fd-13be0a0a9295)
- ![image](https://github.com/user-attachments/assets/e6d5510a-f631-4d62-a0d9-e0b83fd36db0)
- 點兩下
- ![image](https://github.com/user-attachments/assets/4c45d7e3-5d6c-48bd-9ff1-3c649a89c3fd)
- ![image](https://github.com/user-attachments/assets/4c660c3e-3ba0-434d-b710-ba3645105642)
- - 按下`WIN`+`R`輸入`cmd.exe`重新開一個終端介面
- 輸入以下指令確認安裝成功
```
php -v
```
- 應該看到類似以下輸出
```
PHP 8.4.6 (cli) (built: Apr  9 2025 09:45:15) (ZTS Visual C++ 2022 x64)
Copyright (c) The PHP Group
Zend Engine v4.4.6, Copyright (c) Zend Technologies
```


### 2. 安裝Composer
- 官方網址[下載連結](https://getcomposer.org/download/)
- 點擊即可下載
- ![image](https://github.com/user-attachments/assets/166b9380-b2ce-4f77-8bc9-ff5262f17d31)
- ![image](https://github.com/user-attachments/assets/6c4ac39e-0135-4405-9a35-a3fbacd4b9bc)
- ![image](https://github.com/user-attachments/assets/cf352367-a35a-4e82-b307-48373ae8fc12)
- 這個畫面代表 Composer 成功偵測到你安裝好的 PHP 路徑,下一步
- ![image](https://github.com/user-attachments/assets/bab940b5-7d95-454a-b23e-b6b5e37efc55)
- ![image](https://github.com/user-attachments/assets/47c999c0-b4a3-40ab-b279-b3baad13a6b9)
- ![image](https://github.com/user-attachments/assets/23c7bb9e-ac8e-4625-8dee-6a464423c7f2)
- ![image](https://github.com/user-attachments/assets/5ad51df1-0fac-4f96-879c-7d525ad46d39)
- ![image](https://github.com/user-attachments/assets/9a61c825-4888-46a5-90e3-54ed30d2b16a)
- 輸入以下指令確認安裝成功
```
composer -V
```
- 應該看到類似以下輸出
```
Composer version 2.8.8 2025-04-04 16:56:46
PHP version 8.4.6 (C:\php\php-8.4.6-Win32-vs17-x64\php.exe)
Run the "diagnose" command to get more detailed diagnostics output.
```

### 3. 安裝Laravel
- 按下`WIN`+`R`輸入`cmd.exe`
- 輸入以下指令安裝Laravel
```
composer global require laravel/installer
```
- 輸入以下指令
```
laravel --version
```
- 類似以下輸出代表安裝成功
```
Laravel Installer 5.14.2
```
## 新增專案
- 移動到自己像要的目錄底下
- 按下`WIN`+`R`輸入`cmd.exe`
```
laravel new your-project-name
```
- ![image](https://github.com/user-attachments/assets/d4b8d405-11e0-4066-b950-c7a4062b7f76)
- ![image](https://github.com/user-attachments/assets/a89705c6-d6a3-46a6-9950-653652b72ab7)
- 輸入1
- ![image](https://github.com/user-attachments/assets/24dc9647-c393-43a2-8c05-29a61825d914)
- 使用Visual Studio Code來開發laravel專案
- ![image](https://github.com/user-attachments/assets/8f970334-e076-4413-8e72-d9cefde38a58)
```
php artisan serve
```
- 點擊
- ![image](https://github.com/user-attachments/assets/afd67fac-d504-456a-b0d0-ad5ecfce75b8)
- 或瀏覽器url打上
