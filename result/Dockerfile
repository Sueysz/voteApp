# Sélection de la version de l'image Node
FROM node:18.18-alpine3.18
# Choix du répertoire de travail pour le projet
WORKDIR /result
# Copie de tous les fichiers du projet dans le conteneur
COPY . .
# Installation des dépendances avec Yarn
RUN yarn install
# Exposition du port 8888 pour les communications
EXPOSE 8888
# Commande à exécuter pour démarrer l'application
CMD ["node", "server.js"]