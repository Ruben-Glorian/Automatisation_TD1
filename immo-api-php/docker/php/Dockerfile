FROM php:8.4-cli

# updates de base
RUN apt-get update

#extensions docker php a installer
#script pour installer les extension php facilement pour docker
#curl recup la dernière version du script
#chmod our pouvoir l'executer
RUN curl -sSLf \
        -o /usr/local/bin/install-php-extensions \
        https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions && \
    chmod +x /usr/local/bin/install-php-extensions

#Config php
RUN mv "$PHP_INI_DIR/php.ini-development" "$PHP_INI_DIR/php.ini"
RUN install-php-extensions  mysqli pdo_mysql
RUN install-php-extensions @composer
EXPOSE 80