FROM php:7-fpm
# Install modules
RUN apt-get update && apt-get install -y \
	libmcrypt-dev  \
	libicu-dev \
	curl\
	mysql-client \
	&& docker-php-ext-install pdo_mysql \
	&& docker-php-ext-install iconv \
	&& docker-php-ext-install mcrypt \
	&& docker-php-ext-install iconv \
	&& docker-php-ext-install curl \
	&& docker-php-ext-install intl \
	&& docker-php-ext-install gd \
	&& docker-php-ext-install opcache \
	&& docker-php-ext-install mbstring
CMD ["php-fpm"]
