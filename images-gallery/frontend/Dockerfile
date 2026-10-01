FROM node:18-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json ./

RUN npm install --legacy-peer-deps

COPY . ./

CMD ["sh", "-c", "NODE_OPTIONS=--openssl-legacy-provider npm start"]
