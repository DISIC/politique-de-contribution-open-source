---
title: Meilleures Pratiques
layout: default
---

## Meilleures pratiques

### TL;DR

* Gestion des comptes personnels et d'organisations
* Distinction des contributions professionnelles / personnelles
* Aide au choix d'une plateforme de publication
* Aide au choix de la licence
* Diffusion initiale
* Suivi des anomalies
* Tests
* Gestion des versions
* Fichiers par défaut dans un repository
* Headers de fichiers source
* Gestion de la qualité
* Gestion de la communauté

### Gestion des comptes personnels et organisation

Utilisation de repository au sein de comptes d'organisation
Si sur Github, referencer le compte d'organisation comme un compte gouvernemental
Deux propriétaires par repository

### Distinction des contributions personnelles / Professionnelles

Utilisation du compte professionnel avec le mail en ```.gouv.fr```

Créer de repository, configurés de la manière suivante:

* Repository professionnel

`git config user.email <prenom.nom@ministere.gouv.fr>`

* Repository personnel

`git config user.email <email@perso.fr>`

Afin de vérifier que la commande a bien été prise en compte

`git config --get user.email`
