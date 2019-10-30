FROM rust:1.38-alpine3.10

RUN echo "http://mirrors.aliyun.com/alpine/v3.10/main/" > /etc/apk/repositories

RUN apk update && apk add --no-cache git openssh-client expect wget ca-certificates bash make tzdata && \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/myapp

RUN ls
