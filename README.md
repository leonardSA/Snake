# Snake
Projet de SmallTalk  - licence 2 semestre 3 - 2018  
Élève : Joseph Leonard STEPHEN AUGUSTE  
Il s'agit de créer un jeu snake à partir environnement de développement **_Visualworks_**.  

## Classes  

On créer notre application en se basant sur le modèle MVC (Modèle Vue Controlleur), d'où nos classes :
- **Snake** : est notre modèle, c'est dans cette classe qu'est définie notre principal objet ;
- **SnakeController** : notre controlleur qui permettra notamment de changer la direction de notre serpent ;
- **SnakeUI** : est l'interface, ce que l'on voit réellement de notre application ;
- **SnakeView** : s'occupe de l'affichage de notre application dans notre interface.

## Snake  

Variables d'instance | Description
---|---
board | Matrice représentant l'espace de jeu
height | Entier gardant le nombre de lignes de la matrice
width | Entier gardant le nombre de colonnes de la matrice
snake | Collection de points correspondant aux cases sur lesquelles est le serpent
direction | Entier prenant une valeur comprise entre 0 et 3 donnant la direction du serpent (0 haut, 1 droite, 2 bas, 3 gauche)

Méthodes | Description
---|---
initialize | Méthode classique d'initialisation
accessing | L'ensemble des accesseurs 
testBoard | Initialisation de l'objet Snake qui sera utilisé dans notre application

## SnakeController

**_Vide pour l'instant_**

## SnakeUI

Variables d'instance | Description
---|---
playground | La vue de notre application ; elle prend notamment la méthode displayOn qui est définie dans SnakeView afin de nous afficher notre testBoard qui est défini dans Snake
play | Contient le processus lancé lorsque l'on commence à jouer

Méthodes | Description
---|---
initialize | Cette méthode a ici beaucoup d'importance : elle permet d'initialiser le modèle et de permettre l'actualisation de son affichage lorsque celui-ci change
changeBoard | Invalide la vue expirée, ce qui permet la réactualisation de celle-ci
startPlaying | Méthode liée au boutton action permettant de commencer le jeu, elle appelle le processus move
move | Cette méthode fait objet de processus, elle permet uniquement le mouvement de notre serpent et sa mort (lorsqu'il touche un mur) pour le moment
killProcess | Appelé par move lors de la mort du serpent, elle permet de terminer le processus en cours

## SnakeView

Méthode | Description
---|---
displayOn: aGC | Gère l'affichage de notre classe Snake