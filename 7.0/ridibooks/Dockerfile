FROM ridibooks/php:7.0-base
MAINTAINER Koong Kyungmi <kyungmi@ridi.com>

ENV DEBIAN_FRONTEND noninteractive

# Install packages
RUN apt-get update && \

    # Common
    apt-get install -y git unzip

# Install PHP extensions
RUN apt-get install -y php-xdebug php-mysql

# Install Composer
RUN apt-get install -y libcurl4-openssl-dev
RUN curl -sS https://getcomposer.org/installer | php \
    && mv composer.phar /usr/bin/composer
