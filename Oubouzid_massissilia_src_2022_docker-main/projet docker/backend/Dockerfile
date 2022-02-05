
FROM node:10.16-alpine

# Create App Directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install Dependencies
COPY package*.json ./
COPY ./yarn.lock ./

RUN yarn install --silent

# Copy app source code
COPY . .

# Exports
EXPOSE 5000

CMD ["yarn","start"]