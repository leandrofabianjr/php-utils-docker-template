FROM php:7.4-apache
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
RUN echo "xdebug.remote_enable=1" >> /usr/local/etc/php/php.ini
RUN echo "xdebug.extended_info=1" >> /usr/local/etc/php/php.ini
RUN apt-get update
RUN apt-get install -y libpq-dev && docker-php-ext-install pgsql && docker-php-ext-install pdo_pgsql
RUN apt-get install -y libpng-dev && docker-php-ext-install gd
RUN a2enmod rewrite
RUN a2enmod headers

RUN apt-get install -y vim iputils-ping

RUN rm -rf /var/lib/apt/lists/*
