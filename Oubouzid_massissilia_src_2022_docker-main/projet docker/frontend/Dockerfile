# Build react client
FROM node:10.16-alpine

# Working directory be app
WORKDIR /usr/src/app

COPY package*.json ./
COPY ./yarn.lock ./

###  Installing dependencies

RUN yarn install --silent

# copy local files to app folder
COPY . .

EXPOSE 3000

CMD ["yarn","start"]