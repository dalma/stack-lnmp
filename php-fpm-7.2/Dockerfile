####################################
# See: https://hub.docker.com/_/php/
####################################

FROM php:7.2-fpm
MAINTAINER Yuanzhen Zhou <szrednick@gmail.com>

RUN apt-get update \
    && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng-dev libmcrypt-dev \
    && docker-php-ext-install -j$(nproc) iconv \
    && pecl install mcrypt-1.0.1 \
    && docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ \
    && docker-php-ext-install -j$(nproc) gd

RUN docker-php-ext-install -j$(nproc) mysqli
RUN docker-php-ext-install -j$(nproc) zip
