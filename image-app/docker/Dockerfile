FROM sugar708/lara708:php-8

COPY ../../server /var/www/html

# LaravelMixでコンパイルしたいのでCI/CDで実行
# envの前に実行するとよし
RUN npm ci
RUN npm run prod

COPY ../../server/.env.example /var/www/html/.env
