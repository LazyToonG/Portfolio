<h1>S2.01 - Développement d'une application </h1>

<p>On nous a demandé de réaliser un jeu d'échecs, dans le langage de programmation Java,en partant de rien en étant dans un groupe de deux. La difficulté effectivement est qu'on est pas vraiment guidé, certe on nous aide légèrement car il y a certains nom de classe indiqué qu'il faut vraiment mais c'est tout. Dès le début de ce projet on savait qu'il y aurait deux difficultés majeures, le fait qu'il faudra naviguer entre les différentes classes, en l'occurrence on en a fait douze,  et l'affichage car on ne nous a pas appris comment faire une véritable interface graphique. Ducoup malheureusement le résultat n'est pas concluant car il s'agit d'un projet non finit, c'est à dire non exécutable.</p>

<p>Voici un extrait d'une class de nom "Echiquier", plus précisément son constructeur :</p>
```
public class Echiquier {

	private Case[][] echiquier;

	public Echiquier () {
    	for (int i = 0; i< 8; i++){
        	for (int y = 0; y < 8; y++) {
            	echiquier[i][y] = new Case(i,y);
        	}
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

<p>Même si ce projet n'a pas pu aboutir on a pu apprendre dans un milieu difficile, qui nous a forcés à nous creuser le crâne pour voir de la logique cachée à l'horizon. Et bien évidemment cette SAE a pu améliorer notre compétence pour le langage Java.</p>

<p>Extrait de l'énoncé</p>
![Extrait de l'énoncé](https://imgur.com/rw2uScm.png)







