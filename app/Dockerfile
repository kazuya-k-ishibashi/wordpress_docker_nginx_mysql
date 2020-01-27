FROM wordpress:php7.3-fpm-alpine

ARG HOST_GID
ARG HOST_UID

RUN apk update \
  && apk add shadow \
  && groupmod -g ${HOST_GID} www-data \
  && usermod -u ${HOST_UID} www-data \
  && chown -R www-data:www-data /usr/src/wordpress
