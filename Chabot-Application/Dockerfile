FROM python:3.7

RUN apt-get update && apt-get install -yy gcc build-essential python-setuptools

ENV PYTHONUNBUFFERED 1

ADD requirements.dev.txt .
ADD requirements.txt .
RUN pip install -r requirements.dev.txt

WORKDIR /app
