FROM kuborgh/php-shopware:7.0

# Add xdebug
RUN pecl install xdebug-2.5.0 && \
    docker-php-ext-enable xdebug

# replace php.ini with debugging output and xdebug enabled
ADD php.ini /usr/local/etc/php/conf.d/php-ini-overrides.ini
