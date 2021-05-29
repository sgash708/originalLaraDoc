## プロジェクト作成

```zsh
% cd develop
% docker-compose up -d
% docker-compose exec php bash
```
<code>server/</code>配下に作成される

```bash
# Latest(ver8)
$ composer create-project "laravel/laravel" .
# もしくは
$ laravel new hoge
$ vi .env
### ここから ###
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE="develop/.envのMYSQL_DB"
DB_USERNAME="develop/.envのMYSQL_USER"
DB_PASSWORD="develop/.envのMYSQL_PASS"
### ここまで ###

$ php artisan key:generate
$ php artisan config:cache
```

```zsh
% cd ../
% cp -a server/hoge server
```
