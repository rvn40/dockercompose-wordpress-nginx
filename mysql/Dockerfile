FROM mysql:8.0-debian

ENV TZ=Asia/Jakarta

# Add timezone asia/jakarta
RUN apt update -y && apt install -y tzdata curl && \
	ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone && \
	apt-get clean