# TP1 BDD

## La magnificience de la BI

### Qu'est ce que la BI ?

La BI, **Business Intelligence**, est le résultat d'une évolution des besoins de la part des décideurs et analystes des entreprises. Le but du BI est d'aider à la décision et de permettre des analystes précises, complexes et de grande envergure dans les entreprises.

### Différence opérationnel - décisionnel

**Opérationnel** : fait tourner l'entreprises. Assiste le production et le vie quotidienne de celle ci.

* petit volume de donnée à gérer
* utilisé par toute l'entr
* Processus fermés, transactionnels, le but est de donner le moins de marge de manœuvre possible.
* données en lecture/écriture
* réponses très rapide
* niveau de granularité fin
* décentralisés

**Décisionnel** : voit tourner l'entreprise. Permet de générer de la connaissance à partir des données, et donc, d'aider à faire des décisions stratégiques.

* Gros volumes de données à gérer.
* Nombre d'utilisateur restreint (décideurs, analystes).
* Processus ouverts pour permettre la génération de connaissance.
* Données en lecture seule.
* Rapidité moyenne comparée aux systèmes opérationnels.
* Niveau de granularité très grand (on peut avoir des résumés sur ce qui c'est passé durant les 10 dernières années par exemple).
* Centralisés (on veut avoir toutes les données de l'entreprise dans une seule structure).
						
### Entrepôt de données (Data Warehouse)

L'ensemble des données historiées, nettoyées, valides, complètes et cohérentes d'une entreprise. Organisées de tel façon à ce que des non informaticiens puissent en comprendre la structure et l'exploiter, sans l'intervention d'un informaticien.

Les grands du BI (Inmon, Kimball) définissent un entrepôt de données par ses caractéristiques :

* Orienté métier : c'est à dire que dans un entrepôt de données, les informations sont organisées par fonction dans l'entreprise (comptabilité, stocks, ventes, etc.).
* En lecture seule : c'est le point crucial, on ne supprime JAMAIS des données d'un entrepôt puisque sa raison d'exister est de conserver tout changement.
* Organisé en axes : les données sont organisées en axes d'analyses (dimensions) et objets d'analyse (fait). Une dimension est un axe avec lequel nous allons analyser un phénomène dans l'entreprise (fait).
* Intégrées : tous les systèmes stockant des informations dans l'entrepôt sont des sources potentielles de données. Feuilles de calculs, systèmes de production, feuilles de travail, etc. L'entrepôt intégrera ces éléments pour former une vision unique de l'activité de 		l'entreprise.
* Différents niveaux de granularité : l'entrepôt doit être capable de livrer des informations aussi détaillées (ligne de facture) que générales (chiffre d'affaire pour une année), et ce de la façon la plus transparente possible.

###  Dimension en étoile

Utilisée lorsque on a **1 seule table** qu'on découpe pour avoir plusieurs relations, ce qui donne évidemment une étoie1

### Dimension en flocon

Utilisée lorsque on a **plusieurs seule table**, ce qui donne évidemment un flocon