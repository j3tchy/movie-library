FROM mhart/alpine-node:8.15

RUN apk update && apk add bash

WORKDIR /api

RUN npm install express-generator -g --save && npm install nodemon --save-dev && npm install mongoose --save

COPY package*.json /api/

RUN npm install

COPY . /api/

EXPOSE 9000

# TODO: Add wait-for-it.sh
# CMD ["chmod", "+x", "./wait-for-it.sh"]