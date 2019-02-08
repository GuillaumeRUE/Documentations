# MKDocs

[Documentation](https://www.mkdocs.org/) complète

## Installation
[installation](https://www.mkdocs.org/#installation)

## Création de la documentation

Dans un terminal : `mkdocs new <nom_repertoire>`

## Lancement du serveur

* se rendre dans le répertoire de la documentation depuis un terminal

`cd <chemin_vers_le_repertoire>`

* Ecrire la commande

`mkdocs serve`

* La doc est visible [ici](http://127.0.0.1:8000/) une fois le serveur lancé

## Ajout d'une page

* Il faut ajouter un fichier `.md` dans le dossier `docs`
* Ajouter dans le fichier `mkdocs.yml` la ligne :

`- nomPage: <nom_document>.md`

## Changement du thème de la doc

Dans le fichier `mkdocs.yml`, ajouter la ligne :
`theme: readthedocs`

## Création du site HTML

A la racine du dossier de documention, lancer la commande:
`mkdocs build`

Si les liens ne sont pas directs sur les pages HTML, ajouter cette ligne au fichier 'mkdocs.yml':
`use_directory_urls: false` puis relancer un `build`