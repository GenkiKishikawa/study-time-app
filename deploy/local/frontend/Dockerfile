FROM node:22-bullseye

ENV LANG C.UTF-8

WORKDIR /frontend

RUN apt-get update && apt-get install -y \
  vim \
  curl \
  git && \
  apt-get clean && \
  rm -rf /var/lib/apt/lists/*

COPY . /frontend/

RUN npm install yarn
RUN cd react && yarn install && yarn build
