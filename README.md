L'installation d'Openrouteservice se fait via une image Docker, récupérée lors du déploiement décrit dans le fichier `docker-compose.yml` prévu à cet effet.

### Marche à suivre

1. Mettre en place la [gestion des données OpenStreetMap](https://gitlab.avasad.ch/geos/scripts/-/blob/main/README.md)

2. [Installer le reverse proxy NGINX](https://gitlab.avasad.ch/geos/nginx-server/-/blob/main/README.md)

3. Placer le fichier [docker-compose.yml](https://gitlab.avasad.ch/geos/ors/ors-back/-/blob/main/docker-compose.yml) dans le répertoire `/srv/geos/ors-back`

4. Créer le container Docker et déployer l'application

   ```shell
   cd /srv/geos/ors-back
   docker compose up -d
   ```
