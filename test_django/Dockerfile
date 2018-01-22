# Docker Django
FROM python:2.7-alpine

ENV PYTHONUNBUFFERED 1

RUN mkdir /code
WORKDIR /code
COPY requirments.txt /code/
COPY repositories /etc/apk/
RUN  apk update \
  && apk add musl-dev gcc python-dev postgresql-dev \
  && pip install -r requirments.txt -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
ADD . /code/
