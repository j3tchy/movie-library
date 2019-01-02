FROM mhart/alpine-node:8.15

RUN apk update && apk add bash

WORKDIR /app

COPY package*.json /app/

RUN npm install

COPY . /app/

EXPOSE 3000

# TODO: Add wait-for-it.sh
# CMD ["chmod", "+x", "./wait-for-it.sh"]