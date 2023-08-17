FROM node:16.17.0-alpine
RUN apk update && apk upgrade
RUN mkdir /app
WORKDIR /app

COPY package.json /app
COPY yarn.lock /app
RUN yarn install --frozen-lockfile
COPY . .

EXPOSE 3000