# ARG arch
# ARG TARGETPLATFORM=linux/386
# ARG TARGETARCH=linux/386
FROM --platform=linux/386 ubuntu:16.04

LABEL name="Sean"
LABEL email="qtt1536@gmail.com"
LABEL version="1.0"
LABEL description="ubuntu 16.04 32bit for pwn"

#ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul

#RUN apt-get update && apt-get install -y locales && rm -rf /var/lib/apt/lists/* \
    #&& localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
#ENV LANG en_US.utf8

RUN apt-get update && apt-get upgrade -y && apt-get autoremove -y

RUN apt-get install -y file make nasm gcc git curl wget gdb vim zsh ssh netcat

RUN apt-get install -y python python3 python-pip python3-pip python2.7-dev

RUN apt-get install  -y build-essential libssl-dev libffi-dev python-dev libcapstone-dev

# RUN pip install pwn

RUN wget https://bootstrap.pypa.io/pip/2.7/get-pip.py

RUN python3 get-pip.py && rm get-pip.py

RUN pip3 install pwntools

COPY . /app