FROM httpd:2.4

WORKDIR /var/www/html/

COPY server/php.conf /usr/local/apache2/conf/extra/

RUN sed -i \
    -e 's/#LoadModule proxy_module/LoadModule proxy_module/' \
    -e 's/#LoadModule proxy_fcgi_module/LoadModule proxy_fcgi_module/' \
    /usr/local/apache2/conf/httpd.conf \
 && echo "Include /usr/local/apache2/conf/extra/php.conf" >> /usr/local/apache2/conf/httpd.conf

COPY src .
