FROM node:17-alpine
RUN npm install -g pnpm
ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools
RUN apk add make
RUN apk add gcc 
RUN apk add libc-dev
RUN apk add g++