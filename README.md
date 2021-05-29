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

$ php artisan config:cache
$ php artisan key:generate
```

```zsh
% cd ../
% cp -a server/hoge server
```
