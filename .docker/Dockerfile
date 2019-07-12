FROM php:7.2-apache

COPY . /var/www/html
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf

WORKDIR /app

RUN docker-php-ext-install pdo_mysql \
    && chown -R www-data:www-data /var/www/html \
    && a2enmod rewrite
