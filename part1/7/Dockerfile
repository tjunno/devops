FROM ubuntu:16.04

WORKDIR /app
COPY package*.json ./
ENV API_URL='http://localhost:8000'

RUN apt-get update
RUN apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN npm install

COPY . .
EXPOSE 5000
CMD [ "npm", "start" ]