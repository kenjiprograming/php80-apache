FROM php:8.0-apache

RUN apt-get update \
  && apt-get install -y zlib1g-dev libpq-dev mariadb-client git vim zip unzip libzip-dev\
  && docker-php-ext-install zip pdo_mysql mysqli \
  && docker-php-ext-enable mysqli \
  && a2enmod rewrite \
  && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

COPY ./php.ini /usr/local/etc/php/
COPY 000-default.conf /etc/apache2/sites-enabled/
