FROM wordpress:6.3.1-php8.2-fpm-alpine

COPY ./wordpress/config/uploads.ini /usr/local/etc/php/conf.d/uploads.ini
#COPY /path/to/repo/myTheme /var/www/html/wp-content/themes/myTheme

# Add timezone asia/jakarta
RUN apk --no-cache --update add tzdata ca-certificates curl && \
	cp /usr/share/zoneinfo/Asia/Jakarta /etc/localtime && \
	echo "Asia/Jakarta" > /etc/timezone && \
	apk del tzdata