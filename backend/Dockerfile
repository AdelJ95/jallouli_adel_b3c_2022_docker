    FROM node:10.16-alpine

 # Création App Directory
    RUN mkdir -p /usr/src/app
    WORKDIR /usr/src/app
# Installation dépendances 
    COPY package*.json ./
    COPY ./yarn.lock ./

    RUN yarn install --silent

#Copie code de l'application
    COPY . .

#Export

    EXPOSE 5000

    CMD ["yarn","start"]