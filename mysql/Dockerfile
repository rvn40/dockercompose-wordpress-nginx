FROM mysql:8.0-debian

# Add timezone asia/jakarta
RUN apt update -y && apt install tzdata ca-certificates curl && \
	cp /usr/share/zoneinfo/Asia/Jakarta /etc/localtime && \
	echo "Asia/Jakarta" > /etc/timezone && \
	apt-get clean