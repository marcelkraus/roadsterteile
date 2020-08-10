FROM php:7.4-apache

RUN docker-php-ext-install pdo_mysql && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer && curl https://get.symfony.com/cli/installer | bash && mv /root/.symfony/bin/symfony /usr/local/bin/symfony
ADD site.conf /etc/apache2/sites-enabled/000-default.conf
