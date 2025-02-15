# Projet PPII - Semestre S5

## Table des matières
1. [Introduction](#introduction)
2. [Membres du groupe](#membres-du-groupe)
3. [Description du projet](#description-du-projet)
4. [Prérequis](#prérequis)
5. [Installation](#installation)
6. [Exécution](#exécution)

---

## Introduction

Ce projet, réalisé dans le cadre de ma 1ère année à Telecom Nancy.

Bienvenue dans le projet **PPII - Semestre S5**. Ce projet est réalisé dans le cadre du semestre 5 pour l'unité PPII. Vous trouverez ici toutes les informations nécessaires pour comprendre, installer, et exécuter le projet.


## Membres du groupe

- **ALLOMBERT BLAISE Oscar ** - [oscar.allombert-blaise@telecomnancy.eu](mailto:oscar.allombert-blaise@telecomnancy.eu)
- **RAMBEAUX Erwann ** - [erwann.rambeaux@telecomnancy.eu](mailto:erwann.rambeaux@telecomnancy.eu)
- **KAMAL JIT Navjit ** - [navjit.kamal-jit9@etu.univ-lorraine.fr](mailto:navjit.kamal-jit9@etu.univ-lorraine.frm)
- **GODAIL FABRIZIO Giuliana ** - [giuliana.godail-fabrizio1@etu.univ-lorraine.fr](mailto:giuliana.godail-fabrizio1@etu.univ-lorraine.fr)


## Description du projet

Ajoutez ici une description du projet, ses objectifs, et toute autre information pertinente :

- **Sujet :** Application d’analyse et de détection de fuites de données sensibles
- **Objectifs :** Avoir une application capable de détecter la présence de données sensibles dans un document, tout en offrant un historique détaillé des analyses réalisées. L’application attribue également un score aux utilisateurs en fonction du nombre de documents contenant des fuites qu'ils ont publiés.
- **Types de fichiers pris en charge  :** .pdf, .md, .docx, .xlsx, .txt
- **Technologies utilisées :** Python, Flask, HTML, CSS, Bootstrap, Tesseract


## Prérequis

Listez les prérequis nécessaires pour utiliser ce projet (langages, dépendances, etc.) :

- **Langage(s) :** Python 3.11.5, 
- **Frameworks :** Flask, Bootstrap
- **Dépendances :** Voir le fichier `requirements.txt`.
- **Logiciel :** Tesseract


## Installation


### Étapes générales :

1. Clonez ce dépôt :
   ```bash
   git clone https://gibson.telecomnancy.univ-lorraine.fr/projets/2425/ppii-s5/grp29
   cd grp29
   ```
2. Installation de Tesseract:

    Suivre la [documentation](https://tesseract-ocr.github.io/tessdoc/Installation.html)

3. Faites un environnement virtuel : 
    ```bash
    python -m venv venv
    source venv/bin/activate
    ```


4. Installez les dépendances:
    ```bash
    pip install -r requirements.txt
    ```


## Exécution
1. Lancer l'application :

    ```bash
    flask --app index run
    ```
2. Se connecter :
    ```text
        Compte 1:
        antoine.delacroix@gmail.com
        password

        Compte 2:
        marie.dubois@gmail.com
        securepass
    ```

3. Ajouter un document à analyser
4. Cliquer sur le bouton "Analyze"
5. Affichage du résultat de l'analyse
6. Possibilité de voir l'historique des analyses 
7. Partie administration permettant de voir les différents comptes de l'application et les types de données sensibles que l'on cherche dans les documents
8. Possibilité d'ajouter des comptes / des types de données (seulement l'algorithme regex fonctionne dans les ajouts)