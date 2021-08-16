# Tutoriel Express

Bienvenue dans ce tutoriel 👋 nous allons voir comment configurer un serveur avec Express.

## Prérequis

NodeJs doit être installer sur votre ordinateur. Je vous invite à voir <a target="blank" href="https://www.youtube.com/watch?v=lULBx0aXQJc&t=278s">le tuto de la chaîne</a>, pour commencer avec NodeJs.

## Installation
Installation rapide d'un serveur grace à express.
### 1 - Structure de fichier
Créer le fichier `app.js` puis le dossier `public` et le dossier `views`.
### 2 -  Commandes
```js
npm init -y
npm i express
npm install -g nodemon //Si pas déjà installé
```
### 3 - Boilerplate
Ajoutez dans le fichier `app.js`
```js
const express = require('express')
const app = express()
 
app.get('/', function (req, res) {
  res.send('Hello World')
})
 
app.listen(3000)
```
### 4 - Démarrer le serveur
Exécutez la commande 
```
nodemon app.js
```
Ouvrir votre navigateur et aller à l'adresse : 
```
http://localhost:3000/
```