FROM php:8.3-fpm-alpine

WORKDIR /var/www/laratrack

# Установка Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && composer --version

# Установка dev-пакетов для сборки расширений PostgreSQL
RUN apk add --no-cache postgresql-dev

# Установка расширений для работы с PostgreSQL
RUN docker-php-ext-install pdo pdo_pgsql pgsql

# Оставляем контейнер в интерактивном режиме, чтобы он не завершался
CMD ["php-fpm"] 