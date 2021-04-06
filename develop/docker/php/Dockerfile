FROM sugar708/lara708:php-8

RUN apt-get update

COPY conf /usr/local/etc/php/conf.d
COPY 000-default.conf /etc/apache2/sites-available/