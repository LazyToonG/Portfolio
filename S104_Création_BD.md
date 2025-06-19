# S1.04 - Création d'une base de données

Ce projet individuel, plus complexe que les précédents, portait sur la **création et l’alimentation d’une base de données**. Le thème de la base portait sur les **catastrophes naturelles** survenues dans différents pays.

---

## Objectifs de la SAE

L'objectif était de passer par toutes les étapes essentielles à la création d'une base de données :

- Modélisation graphique à l’aide d’un **AGL** (Atelier de Génie Logiciel), avec la réalisation d’un **MEA (Modèle Entité-Association)** ;
- Traduction du MEA en **modèle relationnel** ;
- Création des **tables SQL** correspondantes ;
- **Peuplement des tables**, soit manuellement, soit automatiquement via un fichier de données.

---

## Script SQL de création des tables

Voici un extrait du script SQL utilisé pour créer les tables de la base de données (avec corrections) :

```sql
CREATE TABLE region (
    region_code INTEGER PRIMARY KEY,
    name VARCHAR
);

CREATE TABLE sub_region (
    sub_region_code INTEGER PRIMARY KEY,
    name VARCHAR,
    region_code INTEGER REFERENCES region(region_code)
);

CREATE TABLE country (
    country_code INTEGER PRIMARY KEY,
    name VARCHAR,
    ISO2 CHAR(2),
    ISO3 CHAR(3),
    sub_region_code INTEGER REFERENCES sub_region(sub_region_code)
);

CREATE TABLE disaster (
    disaster_code INTEGER PRIMARY KEY,
    disaster VARCHAR
);

CREATE TABLE disaster (
    country_code INTEGER REFERENCES country(country_code),
    disaster_code INTEGER REFERENCES disaster(disaster_code),
    year INTEGER,
    number INTEGER,
    PRIMARY KEY (country_code, disaster_code, year)
);
```
Ce projet n'était pas vraiment suivi donc on ne nous demandait pas de faire des requêtes précise étape par étape, mais à la place on nous a laissé de l'autonomie avec une consigne assez large. Donc dans ce projet on a vu et mieux compris toutes les étapes de la création d'une table bien que théorique avec les représentations graphique que pratique avec les requêtes de création et de peuplement des tables.

## L'AGL des tables SqL:

![L'AGL des tables SqL](https://imgur.com/dneekMS.png)

