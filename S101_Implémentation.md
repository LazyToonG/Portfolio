<h1>SAE 1.01 - Implémentation</h1>

<p>Dans ce projet universitaire on devait créer une interaction entre des personnes fictives comme dans un réseau social grâce au langage de programmation python en binôme. On devait suivre un énoncé donné qui nous demandais pour chaque question de réaliser des fonctions qui effectue la consigne de la question tel que "Écrire une fonction lecture_reseau_bis(path) prenant en paramètre un chemin vers un tel fichier CSV et retournant un tableau modélisant les interactions entre les personnes du fichier en éliminant les répétitions.", ce qui nous a permis de retourner une fonction de ce style :</p>

```
def lecture_reseau_bis(path):
	< Cette fonction modélise un tableau d'intéractions à
	partir d'un chemin vers un fichier CSV ('path') passé en
	paramètre en éliminant les répétitions d'intéractions.
	Cette fonction retourne le tableau modélisé.

Argument :
	path -- chemin d'accès vers un fichier CSV (chaine de caractères)

	tab_interactions=lecture_reseau(path) #création d'un tableau d'intéractions contenant des répétitions à partir de la fonction 'lecture_reseau'
	tab_final_interactions=[] #création d'un tableau vide que l'on remplira au fur et à mesure
	i=0
	while i<len(tab_interactions):
    	if verification(tab_final_interactions,tab_interactions[i],tab_interactions[i+1]):
    	#vérifie si l'intéraction entre le nom à l'indice i et celui à l'indice i+1 n'est pas
    	#déjà présent dans le tableau 'tab_final_interactions'
        	tab_final_interactions.append(tab_interactions[i])
        	tab_final_interactions.append(tab_interactions[i+1])
    	i+=2 #le tableau d'intéractions ('tab_interactions') est composé de couples de noms, c'est pourquoi on ajoute 2 à l'indice au lieu de 1
	return tab_final_interactions
```
<p>Il y avait en totale 7 questions dans cette SAE mais ce n'est pour autant que c'était simple puisque déjà il fallait faire plusieurs fonctions dans une questions et bien évidemment qu'il fallait réfléchir à la solution de comment réaliser avec du code comment on veut réaliser au résultat voulu.</p>

<p>Lors de cette Sae on nous a fait travailler et améliorer nos compétences sur le langage de programmation python, plus précisément sur le concept des tableaux/liste et dictionnaire pour comprendre et analyser comment les valeurs agissent entre elles.</p>

<p>Voici un extrait du sujet:</p>
![Extrait du sujet](https://imgur.com/F88F2Kb.png)
