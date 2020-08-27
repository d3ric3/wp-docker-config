FROM wordpress:5-fpm-alpine

MAINTAINER Derice <d3ric3@gmail.com>

RUN apk add --no-cache pcre-dev $PHPIZE_DEPS \
        && pecl install redis \
        && docker-php-ext-enable redis.so
