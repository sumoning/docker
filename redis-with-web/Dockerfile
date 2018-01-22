FROM python:2.7-alpine

COPY .pip /root/

RUN mkdir /CODE

COPY app.py /CODE

WORKDIR /CODE

RUN pip install redis flask

CMD ["python","app.py"]
