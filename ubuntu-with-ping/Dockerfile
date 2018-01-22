#ubuntu with ping and ip
FROM ubuntu:16.04

MAINTAINER Su Moning

COPY sources.list /etc/apt/sources.list

RUN apt-get update \
    && apt-get install -y inetutils-ping iproute2 \
    && rm -rf /var/lib/apt/lists/*
