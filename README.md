# frontend-docker

Ce projet est créé pour aider à apprendre les configurations de **docker** pour les projets frontaux.

# Prerequisites

Installez [node](https://nodejs.org/en/download/). 

Exemple d'instructions d'installation de `node LTS 14.x`:

```
curl -sL https://deb.nodesource.com/setup_14.x | bash
sudo apt install -y nodejs
```

Vérifiez votre installation avec `node -v && npm -v`

Installez tous les packages avec `npm install`

## Démarrage en mode production

Notez que toutes les informations ne sont pas nécessaires dans tous les exercices.

## Exo 5 -> pour exécuter le projet


Pour générer et servir en mode production: `npm start`. Cela crée le projet dans un dossier `dist` et le sert dans le port `5000` .

Vous pouvez également créer le projet avec `npm run build` pour créer le projet dans un dossier `dist`, puis le servir comme vous le souhaitez, par exemple:

Pour utiliser un package npm appelé `serve` pour servir le projet dans le port `5000`:

- installer: `npm install -g serve`
- servir: `serve -s -l 5000 dist`

Testez que le projet est en cours d'exécution en allant sur [http://localhost:5000](http://localhost:5000)

## Exo 7 -> pour se connecter au backend

Par défaut, le chemin attendu pour le backend est `/api. C'est là que l'application enverra des demandes. `

Pour configurer manuellement le chemin api exécuté avec `API_URL` la valeur d'environnement définie, par exemple 
`API_URL=http://localhost:8888 npm start` ou `API_URL=<url> npm build`
