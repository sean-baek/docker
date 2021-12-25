# base image is ubuntu 20.04
FROM ubuntu

MAINTAINER Sean <qtt1536@gmail.com>

# 도커 이미지를 생성할 때는 사용자가 입력할 수 없기 때문에 사용자의 입력 없이 넘어가기 위해 설정
# ARG는 docker build시에만 적용되는 변수이며, ENV는 Docker container 내부의 환경변수로 설정된다.
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul

# update, upgrade, package
RUN apt update -y && apt upgrade -y && apt full-upgrade && apt autoremove \
        apt install -y net-tools build-essential make gcc git curl wget gdb vim zsh ssh netcat \
        ruby-full python python3 python3-pip python-dev python3-dev python-setuptools python3-setuptools \
        libssl-dev libffi-dev libc6-i386 libc6-dbg gcc-multilib utils
