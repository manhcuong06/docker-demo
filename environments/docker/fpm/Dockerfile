FROM php:7.2-fpm

RUN apt-get update && \
    apt-get install -y --no-install-recommends git zlib1g-dev zip unzip
RUN docker-php-ext-install zip
RUN curl --silent --show-error https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www/