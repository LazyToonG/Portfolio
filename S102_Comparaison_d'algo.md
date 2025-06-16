<h1>S1.02 - Comparaison d'algo</h1>

<p>Lors de ce projet en binôme on devait programmer des fonctions sous le langage python des algorithmes de tri vu en cours. Pour être plus précis on a vu 4 : le tri à bulle, le tri par insertion, le tri par sélection et le tri rapide. Dans ce projet qui est en réalité la suite du projet S101 (SAE 1.01 - Implémentation), on nous donner des consigne semblable au premier et on devait y répondre mais sa particularité est qu'on devait implémenter un algorithme de tri pour justement trier des utilisateurs fictif et on devait aussi chronométrer nos fonctions pour savoir laquelle est la plus rapide et donc la plus efficace.</p>
<p>Voici un exemple d'une fonction qu'on a créer et qu'on devait chronométrer:</p>
```
from time import * # import de la bibliothèque time

tic = time()   	# top départ

########### Début du traitement à chronométer ###########

def comu_dans_amis(comun,dico):
	groupe=dico[comun[0]]
	tri_popu(groupe,dico)
	for i in groupe:
    	if sont_amis_de(i,comun,dico):
        	comun.append(i)
	return comun

############ Fin du traitement à chronométer ############

tac = time()       	# arrêt du chronomètre

print(round(1000*(tac-tic),2)," ms") 	# on convertit en ms et on arrondit au centième
```

<p>Lors de la réalisation de ce projet on a appréhender le concept de chronométrage d'une fonction/code et la réflexion sur la création d'un code pour permettre un tri efficace tout ça dans le langage de programmation python.</p>

<p>Extrait du travail effectuer pour la SAE 102:</p>
![Extrait du travail effectuer pour la SAE 102](https://imgur.com/8eIOXa2.png)
