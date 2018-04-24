# Snake
Projet de SmallTalk  - licence 2 semestre 3 - 2018  
Élève : Joseph Leonard STEPHEN AUGUSTE  
Il s'agit de créer un jeu snake à partir environnement de développement **_Visualworks_**.  

##Classes
On créer notre application en se basant sur le modèle MVC (Modèle Vue Controlleur), d'où nos classes :
- **Snake** : est notre modèle, c'est dans cette classe qu'est définie notre principal objet ;
- **SnakeController** : notre controlleur qui permettra notamment de changer la direction de notre serpent ;
- **SnakeUI** : est l'interface, ce que l'on voit réellement de notre application ;
- **SnakeView** : s'occupe de l'affichage de notre application dans notre interface.

##Snake
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


