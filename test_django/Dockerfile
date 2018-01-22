# Docker Django
FROM python:2.7-alpine

ENV PYTHONUNBUFFERED 1

COPY .pip /root/
RUN mkdir /code
WORKDIR /code
ADD requirments.txt /code/
RUN pip install -r requirments.txt
ADD . /code/
