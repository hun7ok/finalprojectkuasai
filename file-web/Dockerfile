FROM php:7.2-apache
ENV PHP_EXTENTIONS \
                   mysqli \
                   pdo_mysql

COPY 
RUN docker-php-ext-install $PHP_EXTENTIONS  &&  docker-php-ext-enable $PHP_EXTENTIONS
RUN a2enmod rewrite
RUN service apache2 restart
