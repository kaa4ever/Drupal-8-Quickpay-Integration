FROM php:7.1.5-fpm

# Make sure the files exists in the same location as the NGINX container.
COPY ./webroot /usr/share/nginx

RUN apt-get update && apt-get install -y \
    libpng12-dev \
    && docker-php-ext-install -j$(nproc) mysqli gd opcache pdo pdo_mysql
