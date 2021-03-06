# Skill Quest : Back
# /!\ A lire avant de faire quoi que ce soit /!\
## IMPORTANT
### NE PAS DEVELOPPER SUR LA BRANCHE MAIN MAIS SUR DEVELOP
```
// après le clone du projet
$ git checkout develop
```
### ENSUITE CREER UNE BRANCHE FEATURE SUR LA BRANCHE DEVELOP (C'EST VOTRE BRANCHE PERSO)
```
$ git checkout -b feature_branch
```
### QUAND VOUS AVEZ FINI DE DEV SUR FEATURE, ON MERGE ENSUITE SUR DEVELOP
```
$ git merge feature_branch
```

## Description
Gestion des API, Connexion SGBD

## Config
```
Node             16.13.2
Npm              8.1.2
Express          4.17.2
```

## Proposition de structure
```
src
│   app.js          # Point d'entrée de l'application
└───api             # Contient les controllers des routes pour tous les endpoints de l'application
└───config          # Contient les variables d'environnement et tout ce qui concerne la configuration
└───jobs            # Les tâches récurrentes à exécuter périodiquement
└───loaders         # Séparation en modules des processus qui se lancent au démarrage
└───models          # Entités BD
└───services        # Logique métier
└───subscribers     # Gestion des évènements pour les tâches asynchrones
└───types           # Fichiers de déclarations de types en Typescript

tests
```

## Installation
```
$ cd ../chemin/vers/workspace
$ git clone https://github.com/Skill-Quest-AL3C/skill-quest-back.git
$ cd skill-quest-back
```
## Convention pour les commits
```
<type>: <description>

/!\ Ne pas écrire la description avec des accents, soyez brefs aussi !
```
***
### Type
```
build: changements qui affectent le build ou les dépendances externes (ex: gulp, broccoli, npm)
ci: changements de la conf CI (ex: Travis, Circle, BrowserStack, SauceLabs)
docs: changements concernant la documentation
feat: nouvelle fonctionnalité
fix: correction de bug
perf: amélioration de performance
refactor: un changement dans le code qui n'apporte pas de nouvelle fonctionnalité ni ne corrige de bug
style: changement qui n'affecte pas le fonctionnent du code (ex: espace, formattage de code, points-virgules manquants, etc)
Test: ajout ou correction de tests
```

## Liens utiles
```
Installer les outils : https://www.ganatan.com/tutorials/demarrer-avec-angular
Comprendre l'organisation des branches du git : https://www.atlassian.com/fr/git/tutorials/comparing-workflows/gitflow-workflow
Commencer le dev backend avec node.js : https://softwareontheroad.com/ideal-nodejs-project-structure/#architecture
```
