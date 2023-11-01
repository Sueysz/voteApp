FROM node:18.18-alpine3.18
WORKDIR /result
COPY . .
RUN yarn install
EXPOSE 8888
CMD ["node", "server.js"]