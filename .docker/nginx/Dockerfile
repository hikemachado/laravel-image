FROM nginx:1.15.1-alpine
RUN apk add --no-cache openssl bash

ENV DOCKERIZE_VERSION v0.6.1
RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz
WORKDIR /var/www
RUN rm /etc/nginx/conf.d/default.conf

#COPY ./nginxFIX.conf /etc/nginx/conf.d/nginx.conf

