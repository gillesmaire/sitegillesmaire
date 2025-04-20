---
title: "Les commandes Linux"
date: 2025-04-20
pubtype: "Formation"
description: "Connaître les commandes linux, le shell, la configuration de bash et connaître les grands utilitaires sed ainsi que les commandes pipe. "
tags: ["shell","man","pipe","variables shell","sed"]
weight: 100
duration: 3 jours
---

### CommandesLinux

#### Description

- Apprendre les commandes de base
- Savoir identifier les variables
- Savoir utiliser les ressources d'aide
- Les commandes du bash
- Les grands utilitaires : sed, awk


#### Objectifs

Connaître les commandes linux, le shell, la configuration de bash et connaître les grands utilitaires sed ainsi que les commandes pipe. 

#### Public

- Futurs administrateurs Linux 
- Futurs développeurs Linux 

#### Prérequis

- Aucun

#### Durée

3 jours (21 heures)

#### Moyens techniques 

- Pc sous Linux Debian ou autre distribution

#### Programme


### Journée 1


-  Introduction
    -  Présentation des shells
        - Qu'est ce que le Shell ?
        - Pourquoi le Shell Script ?
        - Comment lancer une commande
        - Exemple de commandes
        - Le shell utile à tous les niveaux
        - Une règle simple
    -  Premières commandes
        - ls :  premiers pas
        - ls : gestion des droits
        - ls -la : affichage autres champs
        - cd
        - Changement de groupe et d'utilisateur
    -  Arborescence
        - Arborescence des fichiers
        - Arborescence mono disque
        - Arbrescence multi disques
    -  Les différents Shell
        - Les différents Shell
        - Types et syntaxes
        - Installation d'un autre shell
-  Aide
    -  L'aide locale
        - Aide : via man
        - Les 9 rubriques des pages man
        - Pages man en français et en couleur(deb)
        - Aide à l'intérieur d'une page de manuel
    -  À savoir
        - Commandes internes au shell
        - Aide pour les commande internes au shell
        - Arguments des commandes
-  Commandes
    -  Accéder au contenu des fichiers 
        - Manipulation  de fichiers : (cp|rm|ln|mv)
        - Affichage du contenu des fichiers texte (cat|more)
        - chmod
        - Taille des fichiers et des répertoires
        - Modifier le propriétaire d'un fichier
    -  Commandes de compression, d'impression et de gestion du temps 
        - Compression/décompression de fichiers
        - Compression/ décompression de répertoires
        - Commandes d'impression 
        - pr 
        - Gestion des répertoires : mkdir
        - Gestion du temps 
    -  Pipe commandes composites et processus
        - Enchaînements de commandes
        - Redirection
        - Affichage des utilisateurs 
        - Gestion des processus
        - Commandes administrateurs système
    -  Commandes diverses
        - Type de fichier
        - Quelques informations système
        - La commande dmesg
        - Ajout d'utilisateur
        - Présentation
        - Connexion par clé ssh
        - Copie et transfert de fichiers sécurisés via SSH

### Journée 2 


-  Variables 
    -  Présentation
        - Les variables utilisées par les programmes
        - Quelques variables multi Shell
        - Quelques variables Bash
        - Fichiers d'environnement des Shells
    -  Variables utilisateur
        - Les variables utilisateur
        - Attention aux caractères blancs
        - Utilisation des variables
        - Portée des variables
        - Remarques sur l'exportation
    -  Prompt
        - Les variables PS
        - Autres variables des champs PS
        - Les commandes ESCAPE
        - Sélection des polices
        - Colorisation de l'invite
    -  Substitutions 
        - Substitution noms de fichiers
        - Substitutions : compléments bash
        - Substitutions complexes en bash
        - Protection des caractères spéciaux
-  Commandes internes au Bash
    -  set
        - help
        - set
        - set -o
        - shopt
        - Options shopt
    -  cd, pushd, popd, umask, type, enable
        - cd
        - pushd
        - umask
        - type
        - enable
        - sortie de shell
    -  Historique  et Alias
        - Historique des commandes (bash)
        - Paramétrage Historique
        - Commandes d'historique
        - echo
        - alias
    -  Commande sur les processus : kill, jobs, wait, ulimit
        - kill
        - Premiers signaux
        - Derniers signaux
        - jobs
        - wait
        - ulimit
    -  Expressions régulières
        - Présentation
        - Caractères
        - Exemples
        - Premiers exemples
        - Captures en Shell
    -  Divers
        - Les tubes nommés
        - setuid
        - Le setgid
        - Le sticky bit
-  Utilitaires 
    -  Commandes cut, tr, uniq, sort, wc, find, grep
        - cut
        - tr
        - uniq
        - sort
        - wc
        - find
        - grep
    -  Commandes de transformation : iconv, od, nl, basename, diff
        - iconv 
        - od
        - nl
        - basename
        - diff
        - head
        - tail
    -  Commande utilitaires : xargs, tee, cmp, comm, paste, sed
        - xargs
        - tee
        - cmp
        - comm
        - paste
        - sed : édition d'un fichier

### Journée 3


-  Awk
    -  Présentation
        - Principe
        - Programme awk
        - Première utilisation
        - La fonction print et printf
        - Définition du séparateur de champs en entrée
        - Définition du séparateur de champs en sortie
        - Définition du fichier de sortie
    -  Invocation 
        - BEGIN END
        - Invocation
        - Script awk avec invocation awk
        - Script awk sans invocation de awk
    -  Instructions
        - Plusieurs instructions
        - if
        - Les opérateurs
        - Condition dans l'affichage
        - Conditions avec regexp
    -  Les variables
        - Les variables système
        - Variables utilisateurs
        - Afficher la valeur de ces variables 
        - Redresser un fichier multilignes
        - Quelques évidences
        - Utilisation de FNR
        - Les types de données manipulées dans awk
        - Calcul dans awk
        - Passage de variables à awk
    -  Les structures de contrôle
        - Boucle
        - Critères de sélection sur test
        - Instructions de contrôle
        - Les fonctions utilisateurs
        - Redirections
    -  Les fonctions
        - Les fonctions awk sur le texte
        - Exemples sur les chaînes


## Exercices

- Découvertes des fichiers d'information système
- Variables par shell
- PS1 et PS2
- S commandes et pipes
- Printf
- Affichage formaté
- Nombre d'utilisateurs utilisant le bash
- Redresser un fichier multilignes



