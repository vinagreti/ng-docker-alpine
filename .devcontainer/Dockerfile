FROM node:12.18.4-alpine3.12

WORKDIR /workspaces/ng-docker-alpine

RUN apk add --update nodejs npm

RUN apk add --update npm

RUN apk add --update git

RUN export CHROME_BIN="/workspaces/ng-docker-alpine/node_modules/puppeteer/.local-chromium/linux-800071/chrome-linux"

RUN echo "PS1='\[\033[01;32m\]\u@\[\033[01;34m\]\W\[\033[00m\]$ '" >> ~/.profile

RUN source ~/.profile

RUN apk update && apk upgrade && \
    apk add --no-cache bash git openssh
