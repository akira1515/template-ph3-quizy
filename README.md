# Qiita
概要はQiitaにまとめております。  
https://qiita.com/ak-posse/items/1921c8b918260697fd12

# パス
- ログイン/新規登録 <br>
localhost 
- ユーザー画面 <br>
/webapp
- 管理者画面表示 <br>
/admin/index




# laravel インストール方法

1. `cd docker`
2. `docker compose build --no-cache` (ビルドする)
3. `docker compose up -d` (コンテナをたてる)
4. `docker compose exec app bash` (app コンテナに入る)
5. `composer create-project --prefer-dist laravel/laravel . "6.*"` (src 配下に laraavel6 をインストール)
6. ブラウザで`http://localhost`にアクセスし、「laravel」が表示されることを確認。

# db接続設定
src/.envを以下のように変更して下さい
```
DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=password
```
<img width="202" alt="スクリーンショット 2022-06-07 16 16 15" src="https://user-images.githubusercontent.com/74942852/172319499-e9457712-e1c6-4f3b-aa64-53a748b39d1a.png">



