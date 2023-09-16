FROM mysql:8.0-debian

ENV TZ=Asia/Jakarta

# Add timezone asia/jakarta
RUN apt update -y && apt install tzdata ca-certificates curl && \
	ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone 