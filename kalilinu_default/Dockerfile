FROM kalilinux/kali-rolling

MAINTAINER Sean <qtt1536@gmail.com>

ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul

RUN apt update && apt upgrade -y && apt autoremove -y && \
        apt install -y docker docker.io kali-linux-headless ssh 

