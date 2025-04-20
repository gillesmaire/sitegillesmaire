---
title: "Linux embarqué sur processeur ARM avec buildroot"
date: 2025-04-20
pubtype: "Formation"
description: "Apprendre à installer une distribution Linux et des développements en compilation croisée sur un équipement ARM au moyen de Buildroot"
tags: ["busybox","buildroot","compilation croisée","qemu"]
weight: 1000
duration: 4 jours
---

### LinuxEmbarqueRaspberryPI

#### Description

Développement Linux embarqué sur carte Carte RaspBery PI

#### Objectifs

Apprendre à installer une distribution Linux et des développements en compilation croisée sur un équipement ARM au moyen de Buildroot

#### Public

- Développeurs

#### Prérequis

- Connaître le C ou le C++
- Connaître les commandes Linux

#### Durée

4 jours (28 heures)

#### Moyens techniques 

- PC sous Linux Debian
    - Pentium I5 ou supérieur
    - 400 Go de disque libre
    - 32 Go de RAM
    - 2 Interface vidéo dont une HDMI 
    - 2 écrans dont un HDMI
    - PC connectés filaires 
    - Box internet avec un port Ethernet libre pour le Raspeberry PI
- Kit Carte RaspBerryPi
    -  version PI2 ou supérieure
    - carte SD 32 Go ou supérieure 
    - lecteur de carte SD sur port USB
    - un clavier USB supplémentaire
    - un cable Ethernet connectable avec la box Internet 

#### Programme


### Journée 1 


-  Présentation
    -  Architecture
        - Architecture Linux
        - Les différents éléments d'un système Linux
        - Le BIOS et le boot
        - Le boot
        - Introduction au Noyau
        - La librairie LibC
    -  Init et démons 
        - Inittab et init
        - Niveau d'exécution
        - Exemple fichier `/etc/inittab`
        - Les différents types de démon
    -  Init et shell 
        - Les commandes de base et programme
        - Le Shell
        - Les gestionnaires de fenêtre
        - Qt
-  Licences 
    -  Les distributions 
        - Les distributions
        - Les outils de mise à jour
        - Organisation du disque
        - Organisation multi disques
        - Hiérarchie sur le disque
        - Répertoire /usr et /var
        - /etc/fstab
    -  Les licences 
        - Objectif
        - Free vs Open Source
        - Avertissement
        - L'objectif
        - Les formes de licence
        - Caractéristiques des licences libres
        - Différences Open source Licences libres
        - Les principales licences de logiciels libres
    -  Différences entre les licences
        - GPL 
        - LGPL 
        - Apache
        - X11 
        - Eclipse 
        - BSD 
        - Licences sur les contenus
-  Compilation 
    -  Compilation des sources
        - Vérification d'intégrité
        - Décompression des sources
        - Git SVN CVS
        - Commandes de base CVS/SVN/git
        - Morphologies des programmes
        - Rappel mécanisme de compilation
        - Les Makefiles
        - Configure
        - Problèmes de compilation
        - Les étapes de compilation
        - Exemples
    -  Les librairies 
        - Le principe des librairies
        - Librairies statiques vs dynamiques
        - Librairies dynamiques
        - Édition de lien
        - Utilisation des librairies
        - Installation d'une librairie sous Debian
    -  La librairie libc
        - Glibc
        - uclibc
        - eglibc
        - dietlibc
        - Newlib

### Journée 2


-  Le noyau
    -  Présentation 
        - Présentation
        - Versions
        - Les sources
        - Configuration du noyau
        - Module / Kernel / None
        - Avantage / Désavantage des modules
        - Commandes sur les modules
    -  Configuration 
        - make xconfig
        - make gconfig
        - make menuconfig
        - make nconfig
        - Autres possibilités
        - Les options de compilation du noyau
        - Options de compilation (fin)
        - Dépendances des options
        - Select
        - Les patches
        - Niveaux de patch
    -  Options de compilation 
        - La compilation
        - Exercice : compiler un noyau
        - Installation du noyau
        - Installation des modules
        - Disque minimal en RAM
        - Fichier config
-  Busybox 
    -  Busybox 
        - Busybox : présentation
        - Busybox : configuration
        - Les commandes Busybox
        - Ajouter des commandes à Busybox
        - Finalisation d'ajout d'une commande
-  Raspberry
    -  Architecture ARM
        - Les processeurs ARM
        - Quelques termes à connaître
        - Les familles de processeurs ARM
        - Les processeurs ARM9 et ARM10 
        - Les Cortex
    -  Présentation de la carte 
        - Les cartes Raspberry
        - Carte Raspberry PI 2
        - Carte raspberry PI 2
        - Légendes
        - OS disponibles
    -  Installation de base 
        - Principe d'installation
        - Copie de Raspbian sur la carte
-  Compilation croisée
    -  Présentation 
        - Compilation croisée
        - Machine Hôte
        - Les compilateurs C et C++
        - Contenu d'une chaîne croisée
        - Les binutils
        - Les librairies de traitement mathématique
        - Les entêtes du noyau
    -  Compilation du compilateur
        - Chaîne de compilation croisée
        - Alternatives à la compilation croisée
        - Les chaînes précompilées
        - Les chaînes de fabrication de cross compilateurs
        - Les composants de la chaîne
        - Processus de fabrication de la chaîne soi-même

### Journée 3 


-  Buildroot
    -  Présentation
        - Utilisation de BuildRoot
        - Schéma de principe
        - Aide
        - Buildroot : principe
        - Paquetages nécessaires à Buildroot
        - Compilation de Buildroot
        - Les paramètres qu'on peut ajouter
    -  Utilisation
        - Exécution
        - Les fichiers générés
        - Les fichiers  .config
        - Utiliser la toolchain générée
        - Utiliser une chaîne de compilation externe
    -  Installation de la distribution
        - Préparation de la carte Micro SD
        - Agrandir la partition à toute la mémoire SD
        - Divers problèmes classiques
        - Le fichier de configuration du lanceur de la Raspberry

### Journée 4 


-  Customisation
    -  Services supplémentaires
        - Connexion sécurisée avec SSH et transferts de fichiers par SCP
        - Serveur httpd de Busybox
        - Ajout d'utilisateurs
        - Ajout de programmes spécifiques
        - Execution de commandes shellScript avant la génération de l'image
        - sed : édition d'un fichier
    -  Paramètres spécifiques
        - Clavier français
        - Configuration de l’ordonnanceur
        - Exemples lignes cron
        - Fichier dtb - uboot - qemu
        - qemu
        - Compiler buildroot pour qemu 
    -  Le kit Raspberry dans QtCreator
        - Ajout de la chaine de compilation dans QtCreator
        - Ajout du device Raspberry
        - Debug croisé avec la Raspberry
        - Connaitre la plateforme destination dans le fichier pro
        - CMake avec buildroot
-  Les fonctions de Gdb 
    -  Techniques de débugage
        - Présentation de gdb
        - Savoir si un exécutable est compilé en mode debug
        - Principe gdb
        - Les commandes pas à pas
    -  Affichage des variables
        - Modification du contexte
        - print variable
        - Autres affichages
    -  Les points d'arrêt
        - gdb : point d'arrêt
        - Breakpoint - watchpoints - catchpoints
        - Watchpoint
        - Gestion des points d'arrêt
        - Break avec liste de commandes
        - Printf dynamique
        - La pile d'appel
    -  Débugage à distance 
        - Debugage du core via Eclipse
        - Debug croisé
        - Installation sur l'équipement distant
        - Mise en route sur l'équipement host
        - Remarques sur le debug croisé
        - Mise en oeuvre sur Eclipse


## Exercices

- Récupérer les sources du jeu Extrême Tux Racer Pro et le compiler
- Construction de la librairie glibc
- Compiler le noyau Linux 
- Compiler Busybox
- Installation d'une image Raspberry PI prête  à l'emploi
- Fabrication d'une Image avec compilation automatique des programmes.
- Fabrication d'une Imageqemu  avec compilation automatique des programmes.



