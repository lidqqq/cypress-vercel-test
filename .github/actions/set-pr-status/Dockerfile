FROM node:slim

# The * after package is there also to copy the
# package-lock.json that should is created when
# you run `npm install.`
COPY package*.json ./

RUN npm ci

COPY action.js /action.js

ENTRYPOINT ["node", "/action.js"]
