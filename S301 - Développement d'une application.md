# S3.01 - Développement d'une application

Lors de cette SAE de 6 personnes, le but était de réaliser un site qui permet de planifier et faire jouer des musiques à distance. Ce projet est visée pour le personelle du magasin pour permettre de mettres des musique de fonds. Il y a trois groupe présent dans le personelle visée, le marketing, le commercial et administrateur. Chaque rôle à ses actions propres, le marketing peut rajouter des musiques surs un planning, le marketing créer des les playlist contenant les musique ou encore rajoute des annonces comme par exemple les promotions et l'administrateur est celui qui modère les deux autres groupe et qui a la possibilité de rajouter un lecteur pour savoir où envoyer le planning avec les musiques ou encore rajouter un utilisateur avec son rôle.  

Ce projet est le plus gros que j'ai reçu et le seul durant le troisème semestre. Et c'est compréhensible, car les tâches demandées n'ont pas été facile et demandait beaucoup d'autonomie pour apprendre de nouvelles connaissance pourle réaliser.

---

## Ennoncer du sujet

> Dans beaucoup d’organisations (entreprises, collectivités, gares, campus…), il faut assurer une diffusion musicale continue, avec insertion de messages publicitaires et possibilité de lancer des messages urgents. L’enjeu est de garantir la continuité de service : même en cas de coupure réseau, il doit toujours y avoir de la musique qui joue. La supervision permet en plus de vérifier que chaque lecteur est bien en fonctionnement et que ses playlists de secours sont correctement synchronisées.

---

## Objectifs du projet


- Suivre l’état des lecteurs (UP/KO),

- Mettre à jour en central la playlist locale et de la synchroniser automatiquement sur les lecteurs,

- Vérifier que la playlist locale de secours est bien à jour,

- Consigner les messages diffusés (musique, publicité, urgent),

- Déclencher des alertes en cas de problème (lecteur KO, playlist obsolète, absence de diffusion).

---

## Les difficultés rencontrées
### Coté groupe :
1. Comprendre la mise en situation de l'énnoncer pour savoir exactement ce qui était demander
2. Se répartir les tâches équitablement entre 6 personnes

### Coté personelle :
1. Trouver des solutions pour résoudre un but
2. Arriver à gérer des membres du groupe qui était passive à l'avancement du projet
3. Arriver à gérer le temps pour rendre le projet à temps
4. DIfficulté matériel, mon ordinateur n'était pas assez puissant pour lancée le code fluidement et rallentissait énorment lors du lancement d'une machine virtuel(qui représente le lecteur)
---

## Compétences techniques utilisées :

- Mise en place des user stories pour la base de donnée
- Création diagramme de cas d’utilisation
- Création du MEA
- Modélisation du schéma relationnel
- Création du répositery Github
- Utilisation du language Python
- Utilisation du micro framwork Flask
- Manipulation d'une base de donnée avec SQL
- Utilisation du protocole SSH (Secure SHell)
- Utilisation du language HTML
- Utilisatin du language CSS
- Utilisation du language JavaScript
- Développement en MVC (Model View Controller)

## Compétences transversales utilisées :

- Création d'un serveur Discord pour qu'on puisse communiquer ensemble et partager des liens/informations
- Agir en tant que chef de groupe (désigné par les autres membres de mon groupe)
- Faire des ajustements finaux d'un cahier des charges
- Création de la matrice RACI
- Documentation régulière de l'avancement du projet dans le journal de bord
- Création d'un diagramme de Gantt théorique réel pour comparé l'avancement

---

## Piste d'améliorations

Je ne peux pas dire que je suis complétement satisfait de la finalité du projet car il manquait certain fonctionnalité tel que la possibilité de mettre récupérer les logs du lecteur. Et aussi Je voulais que le site puisse interagir avec un autre lecteur (ordinateur) au lieu d'une machine virtuelle mais je n'avais pas réussi. Pour améliorer ce projet il faut déja que je me renseigne plus pour trouver une solution de comment trouver un moyen pour que le protocole SSH puisse réellement communiquer avec un autre ordinateur et que je puisse récupérer les logs générer depuis celui-ci.
Je voudrais aussi améliorer les dispositions des boutons concernant les lecteurs en HTML car la dispostion dans ce projet est assez compact est sur une ligne. 

J'ai remarquer qu'a la fin je devais me dépecher de finir mon travail car la date de rendu était proche et dû à cela je n'ai pas pus faire exactement ce que je souhaitais. Pour éviter cela je devrais mieux gérer mon temps, j'ai utiliser beaucoup de mon temps à lire des ocumentation pour trouver ce qu'il me fallait mais maintenant que je sais ça sera bien plus simple pour avancer.

[← Page précédente](S205_Gestion_d'un_projet.md) | [Retour vers le sommaire](A.Sommaire.md)
