# docker-laravel
## setup

- run ```git clone git@github.com:takuya1003/docker-laravel.git```
- run ```cd docker-laravel```
- run ```docker compose up -d --build```
- run ```docker compose exec app bash```
- inside app container, run ```composer install```
- inside app container, run ```cp .env.example .env```
- inside app container, run ```php artisan key:generate```
- inside app container, run ```php artisan storage:link```
- inside app container, run ```chmod -R 777 storage bootstrap/cache```
- inside app container, run ```php artisan migrate```
- open http://127.0.0.1:8080/
 
