FROM php:7.4-apache

# mysqli: the PHP extension the app uses to talk to MariaDB
RUN docker-php-ext-install mysqli

# Non-secret defaults. User and password are injected at runtime, never baked in.
ENV DB_HOST=mysql-service \
    DB_NAME=ecomdb

COPY . /var/www/html/

EXPOSE 80
