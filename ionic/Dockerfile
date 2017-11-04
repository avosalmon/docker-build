FROM node:6.11
MAINTAINER Ryuta Hamasaki "avosalmon@gmail.com"

ENV IONIC_VERSION=3.16.0 \
    CORDOVA_VERSION=7.1.0

RUN npm install -g ionic@"${IONIC_VERSION}" cordova@"${CORDOVA_VERSION}" && \
    mkdir -p /var/app/current

WORKDIR /var/app/current

EXPOSE 8100 35729

ENTRYPOINT ["ionic"]
