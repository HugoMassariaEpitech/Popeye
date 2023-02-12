FROM node:12-alpine

WORKDIR /app/result

COPY --chown=node:node . .

RUN npm install

EXPOSE 80

CMD ["npm", "start"]