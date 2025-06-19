# S2.01 - Développement d'une application

Dans cette SAE, nous avions pour objectif de développer un **jeu d’échecs en Java**, en binôme, **à partir de zéro**. Ce projet représentait un véritable défi, car nous n’étions **pas guidés étape par étape** : seules quelques classes étaient imposées par l’énoncé, mais sans aide sur leur contenu ni sur leur articulation.

---

## Objectifs du projet

Le but était de :

- Travailler en **programmation orientée objet (POO)** ;
- Concevoir un jeu complet, fonctionnel, et modulaire ;
- Gérer les **règles du jeu d’échecs**, le déplacement des pièces, et les interactions entre classes ;
- Développer (si possible) une **interface graphique**, même rudimentaire.

---

## Les difficultés rencontrées

Dès le début du projet, nous avons identifié deux **grandes difficultés** :

1. **La gestion de nombreuses classes interconnectées** (nous en avons créé 12 au total) ;
2. **L’affichage graphique** : aucune notion d’interface graphique ne nous avait été enseignée à ce moment-là.

Malheureusement, nous n’avons **pas pu finaliser le projet**. Le jeu n’est pas exécutable en l’état, mais nous avons tout de même **implémenté une grande partie de la logique du jeu**.

---

## Exemple de code – Constructeur de la classe `Echiquier`

Voici un extrait du constructeur de la classe `Echiquier`, qui initialise toutes les cases et place les pièces selon la configuration d’un jeu d’échecs classique :

```java
public class Echiquier {

    private Case[][] echiquier = new Case[8][8];

    public Echiquier() {
        for (int i = 0; i < 8; i++) {
            for (int y = 0; y < 8; y++) {
                echiquier[i][y] = new Case(i, y);
            }
        }

        // Pièces noires
        echiquier[0][0].setPiece(new Tour("Noir", echiquier[0][0]));
        echiquier[0][1].setPiece(new Cavalier("Noir", echiquier[0][1]));
        echiquier[0][2].setPiece(new Fou("Noir", echiquier[0][2]));
        echiquier[0][3].setPiece(new Dame("Noir", echiquier[0][3]));
        echiquier[0][4].setPiece(new Roi("Noir", echiquier[0][4]));
        echiquier[0][5].setPiece(new Fou("Noir", echiquier[0][5]));
        echiquier[0][6].setPiece(new Cavalier("Noir", echiquier[0][6]));
        echiquier[0][7].setPiece(new Tour("Noir", echiquier[0][7]));
        for (int z = 0; z < 8; z++) {
            echiquier[1][z].setPiece(new Pion("Noir", echiquier[1][z]));
        }

        // Pièces blanches
        echiquier[7][0].setPiece(new Tour("Blanc", echiquier[7][0]));
        echiquier[7][1].setPiece(new Cavalier("Blanc", echiquier[7][1]));
        echiquier[7][2].setPiece(new Fou("Blanc", echiquier[7][2]));
        echiquier[7][3].setPiece(new Roi("Blanc", echiquier[7][3]));
        echiquier[7][4].setPiece(new Dame("Blanc", echiquier[7][4]));
        echiquier[7][5].setPiece(new Fou("Blanc", echiquier[7][5]));
        echiquier[7][6].setPiece(new Cavalier("Blanc", echiquier[7][6]));
        echiquier[7][7].setPiece(new Tour("Blanc", echiquier[7][7]));
        for (int z = 0; z < 8; z++) {
            echiquier[6][z].setPiece(new Pion("Blanc", echiquier[6][z]));
        }
    }
}
```
---
## Compétences acquises même si le projet n’a pas été achevé, il nous a permis de :
- Renforcer notre compréhension de la programmation orientée objet en Java ;
- Apprendre à organiser un projet complexe en plusieurs classes ;
- Travailler sur des structures logiques poussées (gestion de pièces, déplacements, règles de jeu...) ;
- Apprendre à manier GitHub et en même temps le travail en équipe.
- Ce projet nous a poussés à sortir de notre zone de confort et à travailler en autonomie dans un environnement complexe, ce qui est très formateur.
---

## Extrait de l'énoncé
![Extrait de l'énoncé](https://imgur.com/rw2uScm.png)
