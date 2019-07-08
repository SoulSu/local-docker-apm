FROM alpine:latest

LABEL MAINTAINER="soul.sxd@gmail.com"

RUN apk update && \
    apk add libc6-compat 

WORKDIR /

RUN wget https://artifacts.elastic.co/downloads/apm-server/apm-server-6.5.1-linux-x86_64.tar.gz && \
    tar vxf apm-server-6.5.1-linux-x86_64.tar.gz && \
    mv apm-server-6.5.1-linux-x86_64 apm-server

WORKDIR /apm-server

COPY ./apm-server.yml .
