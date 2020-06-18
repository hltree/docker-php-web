FROM php:7.2-apache

RUN docker-php-ext-install pdo_mysql mysqli mbstring && docker-php-ext-enable pdo_mysql mysqli mbstring && a2enmod rewrite
