<h1>S1.04 - Création BD</h1>

<p>Dans ce projet individuel assez complexe on nous demandait de créer et alimenter une base donnée qui se basait sur les différentes catastrophes naturelles sur les différents pays. On devait faire le représentation des tables sur un AGL (Atelier de Génie Logiciel) pour permettre de voir leurs associations entres elles, qui correspond à faire un MEA (modèle entité association). Par la suite on devait faire le peuplement de ces tables manuellement ou bien automatiquement via un fichier.</p>
<p>Voici le script SQL de la création de toute les différents tables :</p>
```
CREATE  TABLE region (
	region_code INTEGER PRIMARY KEY,
	name VARCHAR) ;

CREATE sub_region (
	sub_region_code INTEGER PRIMARY KEY,
	name VARCHAR,
	region_code INTEGER REFERENCES region) ;

CREATE country (
	country_code INTEGER PRIMARY KEY,
	name VARCHAR,
	ISO2 CHAR(2),
	ISO2 CHAR(2),
	sub_region_code INTEGER REFERENCES sub_region) ;

CREATE disaster (
	disaster_code INTEGER PRIMARY KEY,
	disaster VARCHAR) ;

CREATE disaster (
	country_code INTEGER REFERENCES country,
	disaster_code INTEGER REFERENCES disaster,
	year INTEGER,
	country_code,disaster_code,year INTEGER PRIMARY KEY,
	number INTEGER);

```

<p>Ce projet n'était pas vraiment suivi donc on ne nous demandait pas de faire des requêtes précise étape par étape, mais à la place on nous a laissé de l'autonomie avec une consigne assez large. Donc dans ce projet on a vu et mieux compris toutes les étapes de la création d'une table bien que théorique avec les représentations graphique que pratique avec les requêtes de création et de peuplement des tables.</p>

<p>L'AGL des tables SqL:</p>
![L'AGL des tables SqL](https://imgur.com/dneekMS.png)




