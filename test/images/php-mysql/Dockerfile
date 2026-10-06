FROM php:8.5-apache@sha256:72207188ab7ccecc9151f91636368943261c05fb863db7c6af53f37d07ad39eb
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli
RUN apt-get update && apt-get upgrade -y && apt-get -y install systemctl
RUN a2enmod rewrite
