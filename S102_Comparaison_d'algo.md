# S1.02 - Comparaison d'algorithmes

Dans ce projet réalisé en binôme, nous devions programmer différentes fonctions de tri en Python, en lien avec les algorithmes étudiés en cours. Plus précisément, nous avons implémenté **quatre algorithmes de tri** :

- le **tri à bulles**,
- le **tri par insertion**,
- le **tri par sélection**,
- et le **tri rapide** (quicksort).

Ce projet était une **suite logique** du travail effectué lors de la [SAE 1.01 - Implémentation](S101_Implémentation.md), et reprenait une structure similaire, avec des consignes précises à respecter.

---

## Objectif

L'objectif principal était d’**implémenter ces algorithmes** pour trier des **utilisateurs fictifs**, et d’ensuite **mesurer les performances** de chaque fonction afin de déterminer **le tri le plus efficace** selon les cas.

---

## Exemple de fonction chronométrée

Voici un exemple de fonction que nous avons créée et que nous devions chronométrer :

```python
from time import *  # Import de la bibliothèque time

tic = time()  # Début du chronométrage

# -------- Début du traitement à chronométrer -------- #

def comu_dans_amis(comun, dico):
    groupe = dico[comun[0]]
    tri_popu(groupe, dico)
    for i in groupe:
        if sont_amis_de(i, comun, dico):
            comun.append(i)
    return comun

# -------- Fin du traitement à chronométrer -------- #

tac = time()  # Fin du chronométrage

print(round(1000 * (tac - tic), 2), "ms")  # Affichage du temps en millisecondes
```
Lors de la réalisation de ce projet on a appréhender le concept de chronométrage d'une fonction/code et la réflexion sur la création d'un code pour permettre un tri efficace tout ça dans le langage de programmation python.

## Extrait du travail effectuer pour la SAE 102 :

![Extrait du travail effectuer pour la SAE 102](https://imgur.com/8eIOXa2.png)

[← Page précédente](S101_Implémentation.md) | [Retour vers le sommaire](A.Sommaire.md)


