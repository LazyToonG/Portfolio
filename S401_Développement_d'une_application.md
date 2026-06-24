# S4.01 - Développement d'une application

Lors de cette SAE de 5 personnes, le but était de réaliser une application web multi-tenant permettant de planifier et diffuser des musiques à distance sur des lecteurs Raspberry Pi installés dans des entreprises. Ce projet, nommé **MusiQuali**, est destiné au personnel de magasins souhaitant gérer une ambiance sonore. Trois rôles sont présents : le **marketing** qui gère les playlists et les musiques, le **commercial** qui planifie la diffusion sur un planning hebdomadaire, et l'**administrateur** qui gère les utilisateurs et les lecteurs Raspberry Pi.

Ce projet est la continuité directe de la S3.01, mais à un niveau nettement plus avancé. Les fonctionnalités demandées étaient plus complexes, l'architecture plus rigoureuse, et l'autonomie attendue bien plus grande, notamment pour tout ce qui touchait au déploiement réseau et à la communication avec les Raspberry Pi.

---

## Énoncé du sujet

> L'objectif de cette SAE est de terminer le travail entrepris en S3 pour développer un produit fini. De manière à ne pas pénaliser certains étudiants, on peut ne pas repartir de son propre travail s'il n'est pas jugé comme un bon point de départ, et on peut reprendre le travail de S3 d'autres équipes.

---

## Objectifs du projet
 
### Commercial :
- Faire le planning de diffusion musicale
- Ajouter des playlists dans le planning
- Lancer des messages urgents
### Marketing :
- Créer des playlists
- Ajouter et supprimer des musiques
- Voir, rechercher et trier/filtrer les musiques
- Voir, rechercher et trier/filtrer les playlists
- Voir, rechercher et trier/filtrer les messages
### Admin IT :
- Accéder au panel d'administration
- Gérer les utilisateurs (ajouter, supprimer, rechercher, trier/filtrer)
- Modifier le mot de passe des utilisateurs
- Gérer les lecteurs (ajouter, supprimer, rechercher, trier/filtrer)
- Suivre l'état des lecteurs (UP/KO)
- Consulter les logs des lecteurs
### Modérateur :
- Voir toutes les entreprises
- Ajouter et supprimer des lecteurs par entreprise
### Tous les utilisateurs connectés :
- Se connecter à l'application

---

## Les difficultés rencontrées

### Côté groupe :

1. Continuer un projet déja commencer
2. Maintenir une cohérence entre les développements parallèles (frontend, backend, base de données, Raspberry Pi)
3. Gérer les membres moins actifs sans bloquer l'avancement global

### Côté personnel :

1. Comprendre et mettre en place une architecture multi-tenant rigoureuse (isolation des données par entreprise à travers toutes les couches DAO/Service/Controller)
2. Maîtriser la communication SSH et rsync pour déployer les fichiers sur les Raspberry Pi
3. Déboguer des problèmes complexes de synchronisation (fichiers JSON vides reçus côté Raspberry, scripts non déclenchés à distance)
4. Apprendre à gérer correctement les chemins de fichiers en Python pour éviter les bugs selon l'environnement d'exécution
5. Gérer le temps face à la densité des fonctionnalités demandées
6.  Gérer les processus gérer dans les lecteurs
7. gérer les liens entre les informations dans la base de donnée

---

## Compétences techniques utilisées :

- Architecture MVC étendue en DAO / Service / Controller / Templates
- Développement backend en Python avec le micro-framework Flask
- Utilisation de Jinja2 pour l'injection dynamique de variables dans les templates HTML
- Manipulation d'une base de données SQLite avec création automatique des tables
- Développement multi-tenant avec isolation des données par `idEntreprise`
- Utilisation du protocole SSH et de rsync pour le déploiement sur Raspberry Pi
- Génération et déploiement de fichiers de configuration JSON
- Développement d'une API REST (endpoints JSON pour le statut des lecteurs et les logs)
- Utilisation de JavaScript et `fetch()` pour le rafraîchissement dynamique (AJAX)
- Utilisation des langages HTML, CSS et JavaScript côté frontend
- Gestion de logs applicatifs avec un DAO dédié (`INSERT OR IGNORE` pour l'idempotence)
- Utilisation de Git pour le versionnage et la collaboration en équipe
- Utilisation du protocole SSH
- Mise en place du HTTP EN HTTPS

## Compétences transversales utilisées :

- Agir en tant que chef de groupe (désigné par les autres membres)
- Création et suivi d'un diagramme de Gantt théorique et réel
- Rédaction d'un cahier des charges et des user stories
- Création du diagramme de cas d'utilisation et du schéma relationnel (MEA)
- Création d'une matrice des risques
- Documentation régulière de l'avancement dans un journal de bord
- Communication via Discord pour le partage d'informations et de ressources

---

## Piste d'améliorations

Le site et la base de données pourraient être mis en ligne, ce qui était l'un des objectifs que je souhaitais atteindre au début de ce projet, mais que je n'ai pas pu réaliser en raison du manque de temps.  Effectivement, je suis capable de le faire en utilisant mes compétences acquises pendant mon stage. Cependant, si le site est mis en ligne, il sera hébergé gratuitement sur un hébergeur sans nom de domaine.


[← Page précédente](S301_Développement_d'une_application.md) | [Retour vers le sommaire](A.Sommaire.md)
