FROM exozet/php-fpm:7.2.0

RUN docker-php-ext-install exif

#RUN if [-z "$(ls -A /var/www/html)"]; then composer create-project sylius/sylius-standard /var/www/html; fi

#RUN if [ -d /var/www/html ]; then [ "$(ls -A /var/www/html)" ] && echo "Not Empty" || echo "Empty"; fi
#RUN if [ -d /var/www/html ]; then [ "$(ls -A /var/www/html)" ] || composer create-project sylius/sylius-standard /var/www/html ; fi

#FROM php:7.2.7-fpm
#
#RUN apt-get update && apt-get install -y \
#    unzip \
#    zlib1g-dev \ 
#    libicu-dev \
#    libpng-dev \
#    libfreetype6-dev \
#    libjpeg-dev
#
#COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
#
#RUN docker-php-ext-configure gd \
#    --with-freetype-dir=/usr/include/ \
#    --with-jpeg-dir=/usr/include/
#
#RUN docker-php-ext-install \
#  intl \
#  zip \
#  exif \
#  gd \
#  pdo \
#  pdo_mysql
#
#RUN pecl install xdebug
#RUN docker-php-ext-enable xdebug opcache
#
#RUN composer create-project sylius/sylius-standard /var/www/html
#
#COPY php.ini /usr/local/etc/php/conf.d/php.ini
