# Docker Django
FROM python:2.7-alpine

ENV PYTHONUNBUFFERED 1

RUN mkdir /code
WORKDIR /code
ADD requirments.txt /code/
RUN  pip install -r requirments.txt -i http://mirrors.aliyun.com/help/pypi
ADD . /code/
