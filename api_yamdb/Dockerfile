FROM python:3.9-slim as build

WORKDIR /app

RUN apt-get update && apt-get install -y --no-install-recommends build-essential gcc
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . /app
ENV PYTHONUNBUFFERED 1