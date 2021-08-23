# docker-laravel-handson

## reference
https://qiita.com/ucan-lab/items/56c9dc3cf2e6762672f4#docker-compose-%E3%81%A8-docker-compose-%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E3%81%AE%E9%81%95%E3%81%84


## 実行手順
/Users/earthmurakami/Local/PHP/Laravel/docker-laravel-handson
cd docker-laravel-handson
docker compose up -d --build
docker compose exec app bash
composer install
cp .env.example .env
php artisan key:generate
php artisan storage:link
-> http://127.0.0.1:8080
php artisan migrate
exit
