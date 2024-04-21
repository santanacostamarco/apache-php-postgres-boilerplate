FROM php:8.1-fpm-alpine3.18

WORKDIR /var/www/html/

RUN apk --no-cache add \
    git 

COPY composer.json .
# RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
# RUN php -r "if (hash_file('sha384', 'composer-setup.php') === 'dac665fdc30fdd8ec78b38b9800061b4150413ff2e3b6f88543c636f7cd84f6db9189d43a81e5503cda447da73c7e5b6') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
# RUN php composer-setup.php --install-dir=/usr/local/bin --filename=composer
# RUN php -r "unlink('composer-setup.php');"
# RUN composer install

COPY src .




# RUN apk --no-cache add \
#     apache2 \
#     apache2-proxy \
#     php8 \
#     php8-apache2 \
#     php8-common \
#     php8-mbstring \
#     php8-opcache


# RUN ln -sf /dev/stdout /var/log/apache2/access.log \
#     && ln -sf /dev/stderr /var/log/apache2/error.log

# CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]


# FROM php:8.1-fpm-alpine3.18

# WORKDIR /var/www/html


# RUN rc-update add apache2 default
# RUN cat /etc/apache2/httpd.conf

