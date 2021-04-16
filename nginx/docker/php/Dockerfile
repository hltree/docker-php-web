FROM php:7.4-fpm

COPY php.ini /usr/local/etc/php/


RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libmcrypt-dev \
        libpng-dev \
        zlib1g-dev \
        libxml2-dev \
        libzip-dev \
        libonig-dev \
        graphviz \
    && docker-php-ext-install \
        gd \
        pdo_mysql \
        mysqli \
        zip \
