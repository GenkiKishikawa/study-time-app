FROM nginx:1.20-alpine

RUN mkdir /frontend
RUN mkdir /backend


COPY ./deploy/local/nginx/default.conf /etc/nginx/conf.d/default.conf
COPY ./deploy/local/nginx/nginx.conf /etc/nginx/nginx.conf