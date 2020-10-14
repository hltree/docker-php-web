FROM php:7.2-apache

RUN apt-get update && apt-get install -y libfreetype6-dev libmcrypt-dev libjpeg62-turbo-dev libjpeg-dev libpng-dev \
    && docker-php-ext-install iconv mcrypt \
    && docker-php-ext-configure gd \
            --enable-gd-native-ttf \
            --with-freetype-dir=/usr/include/freetype2 \
            --with-png-dir=/usr/include \
            --with-jpeg-dir=/usr/include \
    && docker-php-ext-install gd pdo_mysql mysqli mbstring \
    && docker-php-ext-enable gd pdo_mysql mysqli mbstring \
    && a2enmod rewrite
