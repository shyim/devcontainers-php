FROM php:8.1.12-fpm

COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/
COPY --from=composer/composer:latest-bin / /usr/bin/composer

RUN IPE_GD_WITHOUTAVIF=1 install-php-extensions \
    bcmath \
    bz2 \
    calendar \
    exif \
    gd \
    gettext \
    gmp \
    intl \
    ldap \
    mysqli \
    opcache \
    pdo_mysql \
    pdo_pgsql \
    pgsql \
    soap \
    sockets \
    zip \
    redis \
    amqp



