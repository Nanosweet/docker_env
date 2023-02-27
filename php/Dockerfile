#wersja PHP
FROM php:8.2-fpm


# instalacja composera - menadzera pakietow do PHP
RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
    php composer-setup.php && \
    php -r "unlink('composer-setup.php');" && \
    mv composer.phar /usr/local/bin/composer

# folder roboczy
WORKDIR /var/www


# powstrzymuje autostopa
ARG DEBIAN_FRONTEND=noninteractive 
