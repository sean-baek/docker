FROM xeanbaek/ubuntu20.04_base:1.0

LABEL name="sean"
LABEL email="qtt1536@gmail.com"
LABEL version="1.0"
LABEL description="ubuntu 20.04 web dev base"

# 도커 이미지를 생성할 때는 사용자가 입력할 수 없기 때문에 사용자의 입력 없이 넘어가기 위해 설정
# ARG는 docker build시에만 적용되는 변수이며, ENV는 Docker container 내부의 환경변수로 설정된다.
ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul

RUN apt update && apt upgrade -y && apt autoremove -y

RUN apt install -y php php-gd mariadb-server

COPY . /app

EXPOSE 80 443
