# Blockchain

Ce projet est une implémentation simple d'une Blockchain avec un mécanisme de Proof of Work (PoW). Il permet d'ajouter des transactions, de miner des blocs et de valider la chaîne. 
### Le code du projet se trouve sur la Branche ML.



# Fonctionnalités

✅ Ajouter des transactions à un bloc

✅ Miner un bloc pour l'ajouter à la blockchain

✅ Vérifier l'intégrité de la blockchain (checkChain())

✅ Voir la blockchain complète

✅ Gestion des nœuds réseau (optionnel)



# Installation du projet


📥 Pré-requis

Node.js installé (>= v14)

Git installé



🚀 Installation


Cloner le projet :

git clone https://github.com/fduforest/proof-of-work.git

Se déplacer dans le dossier :

cd proof-of-work

Installer les dépendances :

npm install



🔥 Lancer le serveur


node server.js

Le serveur démarre sur http://localhost:3000.



# Endpoints de l'API

Méthode	Route	Description

GET	/chain	Voir toute la blockchain

POST	/transactions	Ajouter une transaction

POST	/mine	Miner un bloc

GET	/checkChain	Vérifier la validité de la blockchain



# Modifications et Améliorations

✨ Ajouts dans server.js

✔️ Correction des routes (GET /chain, POST /mine, POST /transactions)

✔️ Ajout de checkChain() pour vérifier la validité de la blockchain

✔️ Sécurisation et gestion des erreurs

✔️ Middleware pour gérer les routes inexistantes


✨ Ajouts dans blockchain.js

✔️ Correction du calcul du hash (previousHash)

✔️ Amélioration du mécanisme de Proof of Work

✔️ Vérification complète des blocs (checkChain())

✔️ Gestion des transactions et des blocs



# Tests avec Bruno



Démarrer le serveur (node server.js)

Ouvrir Bruno et tester les endpoints :

GET http://localhost:3000/chain

POST http://localhost:3000/transactions { "sender": "Alice", "receiver": "Bob", "amount": 10 }

POST http://localhost:3000/mine

GET http://localhost:3000/checkChain
