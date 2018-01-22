# Docker Django
FROM python:2.7-alpine

ENV PYTHONUNBUFFERED 1

COPY .pip /root/
COPY sources.list /etc/apt/
RUN mkdir /code
WORKDIR /code
ADD requirments.txt /code/
RUN apt-get update \
  && apt-get install libpq-dev python-dev \
  && apt-get clean all \
  && rm -rf /var/lib/apt/lists/ \
  && pip install -r requirments.txt
ADD . /code/
