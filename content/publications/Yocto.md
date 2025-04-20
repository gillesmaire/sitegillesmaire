---
title: "Linux embarqué sur processeur ARM avec yocto"
date: 2025-04-20
pubtype: "Formation"
description: "Apprendre à installer une distribution Linux et des développements en compilation croisée sur un équipement ARM au moyen de Yocto"
tags: ["linux","yocto","busybox","compilation croisée"]
weight: 1010
duration: 4 jours
---

#### Description

Apprendre à se servir de Yocto	

#### Objectifs

Apprendre à installer une distribution Linux et des développements en compilation croisée sur un équipement ARM au moyen de Yocto

#### Public

- Administrateurs Linux
- Developpeurs Linux

#### Prérequis

C
Shell
CMakeFile

#### Durée

4 jours (28 heures)

#### Moyens techniques 

- Pentium 7  32 Go de RAM 300Go de Disque
- 1 kit RapberryPI + Clavier et écran supplémentaire
- Cable Ethernet

## Programme


### Journée 1 


-  Présentation
    -  Découverte
        - Principe
        - Histoire de Yocto
        - Ressources
        - Les avantages de Yocto
        - Les inconvénients de Yocto
        - Buildroot et Yocto
        - Équipes de travail et choix de la plate-forme
        - Recommandations
        - Dépendances nécessaires sur la machine de développement
        - Les composants de Yocto
        - Choix d'un répertoire de travail
        - Téléchargement de Poky
        - Guide de migration des versions
        - Autres variantes de commandes de chargement
        - Contenu du répertoire poky
    -  Fabrication d'une image 
        - Initialisation de l'environnement de travail
        - Organisation des répertoires build et poky
        - Attention après initialisation
        - Plusieurs répertoires build
        - Lancement du build
        - Processus parallèle bitbake
        - Les différentes états des tâches yocto
        - Test de la machine virtuelle
        - Vérification Busybox
        - Bitbake
        - Les recettes
        - Le répertoire tmp
        - Le fichier local.conf
        - Curiosité dans l'affectation des variables
-  Les variables et layers 
    -  Les variables
        - Les différentes passes de bitbake
        - Comportement de bitbake
        - Expansion des variables
        - Exemples variables
        - OVERRIDES avant la version Honister
        - OVERRIDES après la version Honister
        - Autres variables
        - Les drapeaux de variables
        - La variable IMAGE_INSTALL
        - La variable PACKAGE_EXCLUDE
    -  Les layers
        - Utilisation d'une variable en shell
        - Installation de la couche RapsberryPI
        - Récapitulatif des répertoires
        - Le fichier bblayers.conf
        - Séquence des commandes
        - Exploration du meta raspberrypi
        - Modification de la variable MACHINE dans local.conf
        - Flashage de la carte
        - Remarque sur cette première installation
        - Éléments de vocabulaire
    -  Sélection de paquets
        - Paquets virtuels
        - Versions de paquets
        - Les features
        - Modification du hostname du device
        - Gestion des utilisateurs
        - La directive INHERIT
        - Utilisation de extrausers
        - Les recettes de poky
        - Utilisation d'un package poky
        - Recherche des recettes installées avec devtool
        - Les différentes sources de meta
        - Ajouter une recette extérieure
        - Lister les recettes appartenant à un meta
        - Remarque sur l'organisation du répertoire de travail
        - Création d'une image
        - Customisation de my-image
        - Remarques
-  Fabriquer des recettes
    -  Utilisation de recettes
        - Ajouter une recette
        - Les types de recette
        - Ajouter le fichier bb
        - Renommer la recette bb
        - Les fonction de logging
        - Les variables des recettes
        - Les variables S et B
        - La variable D
        - L'entête d'une recette
        - Les protocoles sources distants
        - Ajout des licences
        - Fichiers licences issus des sources
        - Dépendances des recettes
        - Exploration des dépendances
        - Les tâches d'une recette
        - Installation de fichiers
        - La variable FILES
        - Exécution de la recette
        - Prise en compte de la recette

### Journée 3


    -  Code dans les recettes
        - Intégrer du code Shell dans Bitbake
        - Intégrer du code Python
        - Insérer du code lors de la lecture des fichiers de configuration
        - Processus de création de la recette
        - Fabrication d'une recette avec utilisation de variables
    -  Héritage d'une classe
        - Les classes de Poky
        - Les directives include require inherit
        - Mauvaise fabrication d'une recette utilisateurs
        - Problème avec EXTRA_USERS_PARAMS
        - Utilisation de la classe useradd
        - Recette d'ajout d'un utilisateur
    -  Création d'une recette CMake
        - Fabrication d'une recette CMake
        - La variable SRC_URI
        - Le contenu du fichier hello.tgz
        - Construction de la recette
        - Syntaxe bitbake
        - Points divers sur les recettes
    -  Création d'autres recettes
        - Ajout d'un patch dans une recette
        - Extension de recette pour un fichier patch
        - Utilisation de recipetool
        - Fabrication d'une recette avec devtool

### Journée 4 


-  Configurations
    -  Configuration 
        - Configuration de busybox
        - Configuration du noyau
        - La chaîne compilation SDK et la chaîne de compilation eSDK
        - La chaîne de compilation croisée
        - Plusieurs chaines de compilations croisées
        - Installation du meta-qt5
        - Ajout de la chaine croisée dans QtCreator
        - Mise en place du device
    -  Les tâches
        - Les tâches
        - Gestion des tâches
        - Communiquer avec l'environnement de la tâche de build
        - Drapeaux sur les variables
        - Evènements
        - Extension de classe
        - Dépendances
        - Dépendance récurcive et inter dépendance
    -  Rappel des commandes yocto
        - Commandes bitbake
        - Commandes qemu
        - Commandes bitbake-layers
        - Commandes devtool


### Exercices

- Fabrication d'une image qemu
- Prise en main de la machine ARM en qemu
- Localiser le répertoire générant busybox avant son installation
- Récupérer et installer l'image sur une carte SD pour en vérifier le bon fonctionnement sur la Raspberry
- Choisir une recette extérieure et l'installer sur en qemu et/ou sur votre carte
- EAjouter un utilisateur avec mot de passe sur le device
- Sur les opérateurs
- Ajouter  une programme C dans votre device



