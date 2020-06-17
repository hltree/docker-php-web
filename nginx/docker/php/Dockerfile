FROM php:7.3-fpm

COPY php.ini /usr/local/etc/php/

RUN apt-get update \
    && docker-php-ext-install pdo_mysql mysqli mbstring \
    && docker-php-ext-enable pdo_mysql mysqli mbstring
