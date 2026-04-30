
Retranscrivez ici le résultat de votre conception de l'API REST.

## Liste des *Endpoints*

Pour chacun, préciser :
- requête :
  - URL
  - méthode HTTP
  - en-têtes HTTP
  - paramètres d'URL
  - corps de message (et son format)
- réponse :
  - quelle réponse en fonction des cas ?
  - code de statut HTTP
  - corps de message (et son format)

# Conception

## Suite des actions (Jeu)

-  Se connecter ( authentification )
- Liste Utilisateur
- Connexion à la partie
- Initialiser un partie
  - Liste des bateaux
  - est placé ?
  - Placer les bateaux
  - Deplacer les bateaux
  - tout les bateaux placés ?
- Demarrer la partie ( tire au sort celui qui commence )
- Tirer une torpille
- Checker le board
  - Case déjà jouée
  - Out of bound
  - Raté / touché / Coulé ?
- Fin de partie
- Nouvelle Partie 



## Liste des endpoints

### Utilisateurs
  ```php
    get/users #renvoie tous les utilisateurs
    get/users/{id} # renvoie un utilisateur spécifique 
   ```


### Bateaux
  ```php
    get/ships #renvoie tous les bateaux
    get/ships/{id} # renvoie un bateau spécifique 
   ```

## Liste des fonctionnalités (idées)

- Différents types de missiles ? (missile normal, missile coup double (2 tires), missile zone de dégât (1 cases --> 5 cases en croix X), en colonne  de 3 |, en ligne de 3 _ etc.) 
- Connexion au serveur (avec identification des joueurs ? genre un id ou autres)
- Choix de la taille de la grille
- Choix du nombre de bateau
- A chaque tire, on à une petite probabilité d'obtenir un missile (genre une sorte de loto, imaginons que l'on tire un missile puis on touche aucun bateau, il y aura 1 chance sur 100 par exemple de drop un missile spécial (décrit au dessus))
- Ajout d'un radar ? (faudrais voir si c'est pas trop cheat) --> Découvre une zone de 5 cases en croix (X)

