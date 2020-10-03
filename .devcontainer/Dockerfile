# [Choice] Node.js version: 14, 12, 10
ARG VARIANT=14
FROM node:14.2-alpine

RUN apk update
RUN apk add yarn
RUN yarn global add @vue/cli @vue/cli-service-global
WORKDIR /app
COPY . .
RUN yarn install

EXPOSE 8000
EXPOSE 8080
