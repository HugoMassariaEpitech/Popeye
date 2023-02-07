FROM node:lts-alpine3.17

WORKDIR /app/result

COPY . .

RUN npm install

EXPOSE 80

CMD ["node", "server.js"]