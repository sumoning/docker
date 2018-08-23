FROM python:2.7-slim

WORKDIR /app

ADD . /app

RUN pip install --trusted-host mirrors.163.com -i http://mirrors.163.com/pypi/simple/ -r requirements.txt

EXPOSE 80

ENV NAME Word

CMD ["python", "app.py"]
