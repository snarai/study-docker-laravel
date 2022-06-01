# study-docker-laravel

DockerでLaravel環境を構築する。


## Dockerセットアップ

$ docker-compose build

$ docker-compose up


## Docker環境へログイン

$ docker-compose exec app bash


## ~~composer のインストール~~

~~$ composer install~~


## Laravelプロジェクト作成

$ laravel new laravel 

※プロジェクト名はサンプルです。また、作成した名前に合わせて docker/nginx/default.conf のDocumentRootを変更します。


## ログイン・ログアウト機能を追加

$ composer require laravel/ui --dev

$ php artisan ui vue --auth

$ npm install

$ npm run dev


## ブラウザで表示確認

http://localhost/login


## Duskのインストール

$ composer require --dev laravel/dusk

$ php artisan dusk:install


## Duskのテスト実施

$ php artisan dusk:make LoginTest

※テストケースが /tests/Browser/LoginTest.php に生成される。

$ php artisan dusk

