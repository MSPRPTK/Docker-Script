# Utiliser une image Node.js officielle avec une version spécifique
FROM node:21.7.3

# Définir le répertoire de travail dans le conteneur
WORKDIR /usr/src/app

# Installer git
RUN apt-get update && apt-get install -y git

RUN git clone --branch main https://github.com/MSPRPTK/API_User.git .

# # Installer les dépendances du projet
RUN npm install

# # Exposer le port sur lequel votre application va fonctionner
EXPOSE 3503

# # Définir la commande pour démarrer l'application
CMD ["npm", "start"]
