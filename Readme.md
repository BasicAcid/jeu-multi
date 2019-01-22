# Jeu Multi avec Sockets

## Le projet consiste à proposer un jeu 2 joueurs temps-réel type Pong qui :
- Synchronise les deux machines au démarrage
- Envoi/Lit des messages datés de l'autre joueur pour extrapoler la situation actuelle de jeu

## L'api REST fournie est utilisable comme suit, où k est votre clé d'accès à l'API comme défini dans le fichier joint :
- Aide : GET http://syllab.com/PTRE839/help?k=...
- Ping : GET http://syllab.com/PTRE839/pings?k=...&t0=
- Envoi : POST http://syllab.com/PTRE839/msgs?k=...&to=...&data=... to étant la clé du destinataire et data une chaîne contenant les données
- Réception : GET http://syllab.com/PTRE839/msgs?k=.... Attention, la lecture est bloquante et retire le message de la file

## Livrable
Code source zippé ou lien vers le code source.
