# Dockerfile
FROM node:16.14.0-alpine

# update and install dependency
RUN apk update && apk upgrade
RUN apk add git

# create destination directory
RUN mkdir /app
VOLUME /app
WORKDIR /app

# copy the app, note .dockerignore
RUN corepack enable
RUN yarn install

ENV NUXT_HOST=0.0.0.0
ENV NUXT_PORT=3000

EXPOSE 3000
CMD yarn dev