FROM node:alpine AS base

WORKDIR /usr/src/app

COPY package* ./

RUN npm install

FROM base AS dev

COPY . .

CMD ["npm", "run", "dev"]

FROM base AS prod

COPY . .

RUN npm prune --production

CMD ["npm", "run", "start"]