    FROM node:10.16-alpline

    
    WORKDIR /usr/src/app

    COPY package*.json ./
    COPY ./yarn.lock ./

    RUN yarn install --silent

    COPY . .

    EXPOSE 3000

    CMD["yarn","start"]