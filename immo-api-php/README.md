# Slim 4 API

Simple API using Slim v4 MySQL 
## Run

- Create `.env` from `.env.exemple`
- Update environement variable



## Installation
- Se placer dans la racine du projet (immo-api-php)
- CREER un fichier .env à la racine du projet en se basant sur le fichier .env.exemple
- Lancer `docker compose up`
- Pour avoir les données de la BD, lancer `- Get-Content "immo-api-php/create_db.sql" | docker exec -i immo-api-php-immo-api-php.db-1 mariadb -u admin -padmin immodb`
- http://localhost:8081/ pour l'API