FROM node:22.23.4

WORKDIR /app

COPY package.json ./

RUN npm install

COPY . ./

RUN NODE_OPTIONS=--openssl-legacy-provider npm run build

CMD ["/bin/bash", "-c", "npm run start"]