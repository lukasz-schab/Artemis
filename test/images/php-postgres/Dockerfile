FROM php:8.0-apache@sha256:c87b4c94d53b35520467b6d026f38656ab9a6d446fa3a0fbba1bc633125f9ad2
RUN apt-get update && apt-get upgrade -y && apt-get -y install libpq-dev systemctl
RUN docker-php-ext-install pgsql && docker-php-ext-enable pgsql
