FROM php:7.0.12-fpm


RUN apt-get update -y
RUN echo "deb http://ftp.de.debian.org/debian stretch main" >> /etc/apt/sources.list
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y php7.0-pgsql libpq-dev && docker-php-ext-install pgsql pdo pdo_pgsql

RUN mkdir -p /data
VOLUME ["/data"]
