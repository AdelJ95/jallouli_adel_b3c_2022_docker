    FROM node:10.16-alpline

    RUN mkdir -p /usr/src/app
    WORKDIR /usr/src/app

    COPY package*.json ./
    COPY ./yarn.lock ./

    RUN yarn install --silent

    COPY . .

    EXPOSE 5000

    CMD["yarn","start"]