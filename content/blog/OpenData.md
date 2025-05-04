---
title: "Initiation à l'Open Data"
date: 2025-05-04
draft: false
tags: [Opendata,Velib,Go]
---

### L'open Data

L'Open Data permet d'accéder dans le monde entier à des jeux de données ouverts comme le nombre de vélos sur la borne la
plus proche des chez vous, le nom du bateau que vous voyez au large, la provenance de l'avion que vous voyez dans le ciel
ou des données dans le domaine de la santé, de la démographie etc ...

Ces données sont interrogeables par une interface Web  ou par un programme sachant interpréter les données brutes qui sont au format JSON.

Voici quelques agrégateurs mondiaux de ces jeux de données :
   - https://dataportals.org/
   - http://opendatainception.io/
   - https://data.worldbank.org/
   - http://data.un.org/
   - https://www.fao.org/statistics/en/
   - https://ec.europa.eu/eurostat
   - https://www.data.gouv.fr/fr/



### Exemple d'interrogation d'une station vélib

Pour récupérer les informations concernant la station velib la plus proche de chez vous, allez faire un tour sur  le site https://www.velib-metropole.fr/map#/ et chercher le numéro de la station qui vous intéresse.

On peut également interroger le flux de données de bas niveau en JSON par la requête : https://velib-metropole-opendata.smovengo.cloud/opendata/Velib_Metropole/station_status.json et descendre dans la liste renvoyée jusqu'à la station voulue identifiée par son numéro dans le champs stationCode.
### Exemple de programmation

Voici un petit ShellScript que vous appelez **velib.sh** qui renvoi le nombre de vélos disponibles dans une station. N'oubliez pas d'installer curl et jq sur votre station Linux.

~~~bash
#! /bin/sh
station=$1
URL="https://velib-metropole-opendata.smovengo.cloud/opendata/Velib_Metropole/station_status.json"
curl -s "$URL" | jq ".data.stations[] | select(.stationCode == \"$station\") | .numBikesAvailable"
~~~

Le Shell Script se lance ainsi :

~~~bash
./velib.sh 18034
~~~

Vous pouvez développer aussi en Python, en C++/Qt ou en Go un programme analogue qui affiche en permanence le nombre de vélos
disponibles dans la borne la plus proche de chez vous.

Cet exemple peut être généralisé à des millions de jeux de données collectées en permanence à travers le monde.


