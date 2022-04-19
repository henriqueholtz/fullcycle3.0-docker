# FROM node:alpine3.15
FROM node:slim

WORKDIR /home/node/appnode

COPY index.js .
COPY package*.json .

# USER node
# npm ci is equivalent of "yarn install --frozen-lockfile"
RUN npm ci
CMD ["npm", "run", "start"]