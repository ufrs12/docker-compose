FROM node:18-alpine as build
WORKDIR /app
COPY package*.json /app/
RUN npm ci --omit=dev
COPY . /app/
EXPOSE 3000
CMD [ "node", "server.js" ]
