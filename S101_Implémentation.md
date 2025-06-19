# S1.01 - Implémentation

Dans ce projet universitaire, réalisé en binôme, nous devions créer une simulation d'interactions entre des personnes fictives, à la manière d’un réseau social, en utilisant le langage de programmation Python.  

Nous devions suivre un énoncé précis, dans lequel chaque question nous demandait d’implémenter une ou plusieurs fonctions répondant à une consigne spécifique. Par exemple, l'une des questions nous demandait :  
**« Écrire une fonction `lecture_reseau_bis(path)` prenant en paramètre un chemin vers un fichier CSV et retournant un tableau modélisant les interactions entre les personnes du fichier, en éliminant les répétitions. »**

Cela nous a conduit à développer une fonction telle que :

```python
def lecture_reseau_bis(path):
    """
    Cette fonction modélise un tableau d'interactions à
    partir d'un chemin vers un fichier CSV ('path') passé en
    paramètre, en éliminant les répétitions d'interactions.
    
    Argument :
        path -- chemin d'accès vers un fichier CSV (chaîne de caractères)
        
    Retour :
        Liste d'interactions sans doublons.
    """
    
    tab_interactions = lecture_reseau(path)  # Création d’un tableau d’interactions, possiblement avec des doublons
    tab_final_interactions = []  # Tableau final sans répétitions

    i = 0
    while i < len(tab_interactions):
        if verification(tab_final_interactions, tab_interactions[i], tab_interactions[i+1]):
            # Vérifie si l’interaction entre les deux noms n’est pas déjà dans le tableau final
            tab_final_interactions.append(tab_interactions[i])
            tab_final_interactions.append(tab_interactions[i+1])
        i += 2  # On avance de deux en deux car les interactions sont sous forme de paires
    return tab_final_interactions
```
Il y avait en totale 7 questions dans cette SAE mais ce n'est pour autant que c'était simple puisque déjà il fallait faire plusieurs fonctions dans une questions et bien évidemment qu'il fallait réfléchir à la solution de comment réaliser avec du code comment on veut réaliser au résultat voulu.

Lors de cette Sae on nous a fait travailler et améliorer nos compétences sur le langage de programmation python, plus précisément sur le concept des tableaux/liste et dictionnaire pour comprendre et analyser comment les valeurs agissent entre elles.

## Voici un extrait du sujet :

![Extrait du sujet](https://imgur.com/F88F2Kb.png)

[Retour vers le sommaire](A.Sommaire.md) | [Suivant →](S102_Comparaison_d'algo.md)
