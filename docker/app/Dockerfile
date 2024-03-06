FROM node:20-alpine

WORKDIR /var/www/app
COPY ./app /var/www/app
COPY ./package.json /var/www/app/package.json

RUN apk update && apk add curl

RUN npm install && npm run build


EXPOSE 3000
CMD ["node", "app.js"]
