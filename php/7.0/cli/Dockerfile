# biserantonov/php:7.0-cli
FROM ubuntu:16.04

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
    curl \
    git \
    openssl \
    php7.0 \
    php7.0-cli \
    php7.0-bcmath \
    php7.0-bz2 \
    php7.0-curl \
    php7.0-gd \
    php7.0-intl \
    php7.0-json \
    php7.0-mbstring \
    php7.0-mcrypt \
    php7.0-mysql \
    php7.0-soap \
    php7.0-zip \
    php-imagick

# Set up the volumes and working directory
VOLUME ["/app"]
WORKDIR /app

# Set up the command arguments
ENTRYPOINT ["php"]
CMD ["-v"]