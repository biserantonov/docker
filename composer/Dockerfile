# biserantonov/composer:7.0
FROM biserantonov/php:7.0-cli

RUN apt-get update && apt-get install -y wget openssh-client mercurial

ENV PATH /composer/vendor/bin:$PATH
ENV COMPOSER_ALLOW_SUPERUSER 1
ENV COMPOSER_HOME /composer

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN chmod -R 777 /composer

ENTRYPOINT ["composer"]
CMD ["-"]
