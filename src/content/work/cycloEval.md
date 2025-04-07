---
title: CycloEval
publishDate: 2025-01-20
img:  /assets/cycloEvalecran.png
img_alt: l'image du site
description: |
  CycloEval est un projet visant à analyser les données de capteurs provenant de smartphones sur un vélo pour évaluer les conditions de conduite et détecter les chocs. Le projet utilise une combinaison de technologies pour collecter, traiter et visualiser les données.
tags: 
   - React
   - Python
   - Endpoints
   - CI/CD
   - Cloud 
---

### CycloEval

##### Description
CycloEval est un projet visant à analyser les données de capteurs provenant de smartphones sur un vélo pour évaluer les conditions de conduite et détecter les chocs. Le projet utilise une combinaison de technologies pour collecter, traiter et visualiser les données.

##### Fonctionnalités
- Collecte de données : Utilisation de l'application Sensor Logger pour enregistrer les données des capteurs.
- Traitement des données : Analyse des données de capteurs pour détecter les chocs et évaluer les conditions de conduite.
- Visualisation : Affichage des trajectoires et des chocs sur une carte interactive.

##### Prérequis
- Node.js 18+ et npm (ou pnpm)
- Python 3.8+
- pip

##### Installation

**Frontend :**

1. Naviguez vers le répertoire `client` :
 
cd client
 
2. Créez un fichier `.env` avec le contenu suivant :
 
VITE_API_URL=http://localhost:8000
 
3. Installez les dépendances :
 
npm install
 
4. Démarrez le serveur de développement :
 
npm run dev
 

**Backend :**

1. Installez les dépendances Python :
 
pip install -r server/requirements.txt
 
2. Démarrez le serveur FastAPI :
 
uvicorn server.main:app --host 127.0.0.1 --port 8000 --reload
 

**Server Setup :**

Vous pouvez utiliser le script `deploy.sh` ou relancer manuellement les services.

- Pour redéployer le projet :

docker-compose down
docker-compose up --build -d

- Pour forcer le redéploiement (cette opération supprimera la base de données) :

docker-compose down
docker-compose up --build --force-recreate -d


- Vérification de l'état :
  - Pour le CI/CD et le webhook :
    tail -f local_api.log
  - Pour consulter les logs du backend et du frontend :
    docker logs fastapi_backend
    docker logs vite_frontend

Avant toute modification, assurez-vous de consulter les Dockerfiles des dossiers `server` et `client`, le fichier Docker Compose ainsi que le dossier Nginx. Testez toujours avec `npm run build` et `npm run dev` avant de pousser vos changements pour éviter de casser le pipeline CI/CD.

Enjoy ;)
