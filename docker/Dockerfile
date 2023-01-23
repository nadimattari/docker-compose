FROM php:8.0-apache

RUN apt-get update && apt-get install -y libzip-dev \
	&& docker-php-ext-install -j$(nproc) pdo_mysql session zip

WORKDIR /var/www/html
