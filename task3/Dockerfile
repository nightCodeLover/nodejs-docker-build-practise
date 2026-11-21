FROM node:16-alpine

WORKDIR /usr/src/app

COPY packages/package*.json ./

RUN npm i --omit=dev

COPY src/* ./

EXPOSE 3032

ENTRYPOINT ["node", "main.js"]