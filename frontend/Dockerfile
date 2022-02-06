    
    # Client 
    FROM node:10.16-alpline
    
    # Espace de travail directory de l'application
    WORKDIR /usr/src/app

    COPY package*.json ./
    COPY ./yarn.lock ./

# Install des dépendances 
    RUN yarn install --silent


# Copie des fichiers locaux 

    COPY . .

    EXPOSE 3000

    CMD["yarn","start"]