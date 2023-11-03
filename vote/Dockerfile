# Sélection de la version de l'image Python
FROM python:3.11.6-alpine3.18
# Choix du répertoire de travail pour le projet
WORKDIR /vote
# Copie de tous les fichiers du projet dans le conteneur
COPY . .
# Installation des dépendances à partir du fichier 'requirements.txt' en utilisant pip
RUN pip install -r requirements.txt
# Exposition du port 8080 pour les communications
EXPOSE 8080
# Commande à exécuter pour démarrer l'application
CMD ["python", "app.py"]