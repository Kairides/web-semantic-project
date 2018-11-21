# Web semantic project

This project is part of our 'Web Semantic' module. 

* [Etape 1](https://github.com/RoxaneKM/web-semantic-project/edit/master/README.md#etape-1) 
* [Etape 2](https://github.com/RoxaneKM/web-semantic-project/edit/master/README.md#etape-2)

## Consignes projet 
* [Consignes](https://docs.google.com/document/d/1QL7D6zpCqcbWIOy2oitHO7SfcmTnf1Ps1ncrEOEwWZE/edit)
* [Slides de tout les groupes](https://docs.google.com/document/d/1LE7Jh_jwyxZoCOW7hc7caXb946pYNszV1U9HiaZ6nQA/edit)

## Rendu
* [Diapo hapinness report](https://docs.google.com/presentation/d/1xv-MBmoSdE04zFjmj5UKY_AnCqqhu3dZnK-nblnLPl4/edit)

## Dataset 
* Source du dataset : [https://www.kaggle.com/unsdsn/world-happiness](https://www.kaggle.com/unsdsn/world-happiness)

### *NEW UPDATE* : Années 2015, 2016 et 2017
* [Dataset format au format CVS](https://github.com/RoxaneKM/web-semantic-project/blob/master/happiness.csv)
* [Dataset au format ttl](https://github.com/RoxaneKM/web-semantic-project/blob/master/happiness2.ttl)
* [Mapping sparql](https://gitlab.com/RoxaneKM/web-semantic-project/blob/master/mapping2.rq)

### Année 2017 (uniquement)
* [Dataset format au format CVS](https://github.com/RoxaneKM/web-semantic-project/blob/master/2017.csv)
* [Dataset au format ttl](https://github.com/RoxaneKM/web-semantic-project/blob/master/happiness.ttl)
* [Mapping sparql](https://gitlab.com/RoxaneKM/web-semantic-project/blob/master/mapping.rq)

### Commande conversion (windows)
* Commande linux : `tarql mapping.rq >happiness.ttl`
* Pour convertir en utf-8 (si besoin): `Get-Content .\rdf.ttl | Set-Content -Encoding utf8 rdf-utf8.ttl`

## Etape 1

### Requêtes Sparql

#### 1. Top 10 : Most happy countries
* [Lien code](https://github.com/RoxaneKM/web-semantic-project/blob/master/rank_most_important.rq)
* Commande windows : `sparql.bat --query top10.rq >top10.txt`
* Commande linux : `sparql --query top10.rq >top10.txt`

#### 2. Rank most important
* [Lien code](https://github.com/RoxaneKM/web-semantic-project/blob/master/top10.rq)
* Commande windows : `sparql.bat --query rank_most_important.rq >rank.txt`
* Commande linux : `sparql --query rank_most_important.rq >rank.txt`

## Etape 2

### Liaison avec d'autres datasets

* Lien avec [dataset tsunamis](https://github.com/RoxaneKM/web-semantic-project/blob/master/tsunami.ttl)
* Lien avec [dataset volcano](https://github.com/RoxaneKM/web-semantic-project/blob/master/volcano.ttl)

### Requêtes liant les 3 datasets

#### Le rang des pays ayant eu des tsunamis ou des volcanos

* [Lien code](https://github.com/RoxaneKM/web-semantic-project/blob/master/catahappiness.rq)
* Command windows : `sparql.bat --query catahappiness.rq >catahappiness.txt` 
* Command linux : `sparql --query catahappiness.rq >catahappiness.txt` 

#### Le rang des pays ayant eu des tsunamis ou des volcanos en 2017
* [Lien code](https://github.com/RoxaneKM/web-semantic-project/blob/master/catahappiness2017.rq)
* Command windows : `sparql.bat --query catahappiness2017.rq >catahappiness2017.txt` 
* Command linux : `sparql --query catahappiness2017.rq >catahappiness2017.txt` 
 
