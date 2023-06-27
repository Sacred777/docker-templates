FROM php:8.2-apache

RUN apt-get update && apt-get install -y wget git unzip \
    && pecl install xdebug-3.2.1 \
    && docker-php-ext-enable xdebug

RUN wget https://getcomposer.org/installer -O - -q \
    | php -- --install-dir=/bin --filename=composer --quiet

WORKDIR /var/www/html
