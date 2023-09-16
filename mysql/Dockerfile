FROM mysql:8.0-debian

# Add timezone asia/jakarta
RUN apt update -y && apt install ca-certificates curl && \
	DEBIAN_FRONTEND=noninteractive TZ=Etc/UTC+7 apt install tzdata && \
	apt clean