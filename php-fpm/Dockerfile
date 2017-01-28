FROM php:7.1.0-fpm-alpine

MAINTAINER Ramzi Ameur <double.ramzi@hotmail.com>

RUN apk add --update --no-cache \
    icu-dev \
    freetype-dev \
    libjpeg-turbo-dev \
    libpng-dev

RUN docker-php-ext-install pdo pdo_mysql opcache intl

COPY double-gestion.project.ini /usr/local/etc/php/conf.d
COPY double-gestion.project.pool.conf /etc/php7/fpm.d/

WORKDIR /var/www/double-gestion.project