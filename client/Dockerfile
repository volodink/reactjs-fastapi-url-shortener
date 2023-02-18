FROM node:16-buster

WORKDIR /client

COPY package.json .
COPY package-lock.json .

RUN npm install

COPY src ./src
COPY public ./public
COPY tsconfig.json .

CMD ["npm", "start"]
