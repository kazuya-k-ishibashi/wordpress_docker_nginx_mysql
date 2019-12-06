FROM wordpress:php7.3-fpm-alpine

RUN apk update
RUN apk add shadow

RUN groupmod -g 1000 www-data \
  && usermod -u 1000 www-data \
  && chown -R www-data:www-data /usr/src/wordpress

