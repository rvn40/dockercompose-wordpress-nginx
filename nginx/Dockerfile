FROM nginx:alpine3.18

COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
# COPY ./nginx/ssl/chain.pem /etc/ssl/chain.pem
COPY ./nginx/ssl/fullchain.pem /etc/ssl/fullchain.pem
COPY ./nginx/ssl/privkey.pem /etc/ssl/privkey.pem

# Add timezone asia/jakarta
RUN apk --no-cache --update add tzdata ca-certificates curl && \
	cp /usr/share/zoneinfo/Asia/Jakarta /etc/localtime && \
	echo "Asia/Jakarta" > /etc/timezone && \
	apk del tzdata