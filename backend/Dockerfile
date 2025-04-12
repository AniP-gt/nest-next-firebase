FROM node:22.14-slim

WORKDIR /app

RUN apt-get update && \
  apt-get upgrade -y && \
  apt-get install -y --no-install-recommends \
  curl

ENV LANG=ja_JP.UTF-8
ENV TZ=Asia/Tokyo

COPY . .

EXPOSE 4000

