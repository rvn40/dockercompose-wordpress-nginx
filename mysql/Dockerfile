FROM mysql:8.0-debian

# Add timezone asia/jakarta
RUN apk --no-cache --update add tzdata ca-certificates curl && \
	npm install --legacy-peer-deps && \
	cp /usr/share/zoneinfo/Asia/Jakarta /etc/localtime && \
	echo "Asia/Jakarta" > /etc/timezone && \
	apk del tzdata