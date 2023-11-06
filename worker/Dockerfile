# Utilisation de l'image SDK .NET Core 7.0
FROM mcr.microsoft.com/dotnet/sdk:7.0-alpine
# Choix du répertoire de travail pour le projet
WORKDIR /worker
# Copie de tous les fichiers du projet dans le conteneur
COPY . .
# Restauration des dépendances du projet .NET
RUN dotnet restore
# Publication de l'application en mode "release" sans restauration des dépendances
RUN dotnet publish -c release --self-contained false --no-restore
# Commande de démarrage de l'application, spécifiant le chemin de l'exécutable
CMD ["dotnet", "bin/release/net7.0/Worker.dll"]