---
title: Bonnes pratiques
menuName: pratique
---

## En résumé

* Utilisation nécessaire d'un système de suivi de version distribué (git, bitkeeper, mercurial) 
* Aide au choix d'une plateforme de publication
* Gestion des comptes personnels et d'organisation
* Inventaire des comptes d'organisation
* Distinction des contributions professionnelles / personnelles
* Aide au choix de la licence
* Gestion des versions
* Fichiers par défaut dans un dépôt (repository)
* Entêtes (headers) de fichiers sources
* Traçabilité des développements (DCO)
* Outillage

## Système de suivi de version

L'utilisation d'un système de suivi de version distribué tel que git est recommandée. Les systèmes svn ou cvs sont déconseillés.

## Partage du code source sur une plateforme Web

En plus du système de suivi de version du code source, une plateforme Web propose une panoplie d'outils collaboratifs associés et vise à mobiliser une communauté de développeurs.  Ces plateformes peuvent être hébergées par un tiers ou par l'administration.

Exemples de plateformes Web hébergées par un tiers :

 * Github : https://github.com
 * Gitlab : http://gitlab.com (version entreprise)
 * Framagit : http://framagit.org - utilisant [Gitlab](https://about.gitlab.com/installation/)
 * Adullact : http://gitlab.adullact.net - utilisant [Gitlab](https://about.gitlab.com/installation/)
 * FSFE : https://git.fsfe.org - utilisant [Gitea](https://gitea.io/)
 * FSF : https://git.savannah.gnu.org/cgit/ - utilisant [cgit](https://git.zx2c4.com/cgit/)

Le code source de github.com n'est pas libre tout comme certains modules de gitlab.com ; certaines plateformes publient des données anonymisées en open data ; leurs portées géographiques peuvent varier, de même que le nombre de développeurs qui l'utilisent.  La liste est incomplète.

Le choix de créer un compte d'organisation au sein d'une plateforme Web existante relève de l'administration, qui peut également héberger sa propre forge publique.

Le positionnement d'un projet sur une forge doit se faire en fonction du niveau de collaboration attendu et des interfaces avec les dépots privés et le reste de la plateforme de développement.

## Gestion des comptes personnels et d'organisation

Utilisation de dépôts au sein de comptes d'organisation. Les dépôts de comptes personnels sont à proscrire et ne doivent
être utilisés que pour des développements personnels.
 
Il est recommandé d'avoir deux propriétaires (owner) par dépôt.

## Inventaire des comptes d'organisation

Des réflexions sont en cours sur la capacité de proposer un inventaire automatique tant du point de vue des dépôts
d'organisation que de l'inventaire des services.

> Pour référencer le compte d'organisation comme un compte gouvernemental dans Github :
>
>  * Inscrivez vous si ce n'est pas déjà fait dans la communauté [https://github.com/government/welcome](https://github.com/government/welcome)
>  * Référencez votre compte d'organisation en l'ajoutant sur la page : [https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml](https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml) conformément à la page [https://government.github.com/community/](https://government.github.com/community/)

## Distinction des contributions personnelles / professionnelles

Utilisation du compte professionnel, par exemple avec un mail en ```.gouv.fr``` ou ```.cnrs.fr```.

Créer le dépôt, configuré de la manière suivante :

* Dépôt professionnel

`git config user.email <prenom.nom@ministere.gouv.fr>`

* Dépôt personnel

`git config user.email <email@perso.fr>`

Afin de vérifier que la commande a bien été prise en compte :

`git config --get user.email`

Les pseudonymes sont gérés de la même manière. Une adresse électronique (ou alias) doit donc être mise à disposition par le ministère pour permettre l'utilisation du pseudonyme.

## Aide au choix de la licence

Le choix d'une licence est aussi le choix d'une communauté de développeurs et d'un écosystème d'outils associés. Une fois la famille de licence trouvée, c'est avant tout la communauté visée qui détermine le choix.

Les licences recommandées par défaut sont :

  * Permissive : Apache 2.0
  * Avec obligation de réciprocité : GNU GPL v3 (standard, lesser ou affero en fonction)

 > Multilicensing : il est possible de fournir un logiciel sous plusieurs licenses simultanément, bien que cela puisse entraîner de la confusion.

## Gestion des versions

Avoir une politique de gestion des versions est recommandé. Le guide de versioning sémantique (https://semver.org/lang/fr/) est un bon exemple à suivre.

## Fichiers présents dans le dépôt

Assurez-vous d'avoir au minimum les fichiers README, CONTRIBUTING et LICENSE.

* README : description du projet. Peut décrire l'objectif et l'administration à l'origine de la publication.

* CONTRIBUTING : guide de contribution, comment s'impliquer et identification du processus de contribution et des licences associées. Exemple: [https://github.com/moby/moby/blob/master/CONTRIBUTING.md](https://github.com/moby/moby/blob/master/CONTRIBUTING.md)

* LICENSE : licence de publication du logiciel.

* MAINTAINERS : liste des mainteneurs du projet (avec des droits de vote ou de commit généralement). Exemple: [https://github.com/moby/moby/blob/master/MAINTAINERS](https://github.com/moby/moby/blob/master/MAINTAINERS)

* ROADMAP : feuille de route publique.

* CONDUCT : un code de conduite pour réguler la communauté de contributeurs. Des exemples peuvent être trouvés :  [https://www.djangoproject.com/conduct/](https://www.djangoproject.com/conduct/) et [https://github.com/18F/code-of-conduct](https://github.com/18F/code-of-conduct).

* GOVERNANCE : décrit la gouvernance du projet, les rôles et les drois de votes. Un exemple est disponible dans ce dépôt [gouvernance.md]({{< relref "gouvernance.md" >}})

* NFR : choix d'architecture technique du projet qui ne correspondent pas à des exigences fonctionnelles.

Ces fichiers doivent être en texte simple ou avec du marquage minimum (ie Markdown). Il n'est pas recommandé d'utiliser des formats binaires (ie PDF)

## Entête des fichiers sources

Conformément aux recommandations détaillées dans [https://software.reuse](https://software.reuse) chaque fichier de code source
doit disposer de son auteur, de son identifiant de licence SPDX, ainsi que d'une copie de la licence dans le repository local.

  *  Exemples d'entête de fichier (headers) :

```
 /*
  * Copyright (c) 2017 Alice Commit <alice@example.com>
  * 
  * SPDX-License-Identifier: BSD-2-Clause
  * License-Filename: LICENSES/BSD-2-Clause_Alice.txt
  */

```

ou dans le cas d'un projet faisant un suivi automatique de ses contributeurs :

```
 /*
  * This file is part of project X. It's copyrighted by the contributors
  * recorded in the version control history of the file, available from
  * its original location http://git.example.com/X/filename.c
  * 
  * SPDX-License-Identifier: BSD-2-Clause
  * License-Filename: LICENSES/BSD-2-Clause_Charlie.txt
  */
```

Ces identifiants permettent de générer automatiquement des inventaires des licences sous la forme de « Bill of Material », afin de
garantir la conformité du logiciel.

L'ensemble des identifiants SPDX est disponible à cette adresse : [https://spdx.org/licenses/](https://spdx.org/licenses/)

## Traçabilité des developpements (DCO)

Afin de garantir l'origine des contributions soumises, la mise en œuvre d'un Developer's Certificate of Origin est recommandée.  
Une traduction française est mise à disposition [DCO-Fr.txt](https://github.com/DISIC/politique-de-contribution-open-source/blob/master/DCO-fr.txt)

Pour l'instant, le sign-off ne se fait qu'en anglais en utilisant la commande

`git commit --signoff`

## Bonnes pratiques de développement

 * Ecrire du code lisible et intelligible
   * choisir (pour un nouveau projet) et respecter une unique
     convention de développement (*coding style*) au sein d'un même projet
     * [https://github.com/google/styleguide](https://github.com/google/styleguide)
     * [https://www.gnu.org/prep/standards/](https://www.gnu.org/prep/standards/)
     * [https://www.kernel.org/doc/Documentation/process/coding-style.rst](https://www.kernel.org/doc/Documentation/process/coding-style.rst)
     * [http://www.php-fig.org/psr/psr-2/](http://www.php-fig.org/psr/psr-2/)
     * [http://pear.php.net/manual/en/standards.php](http://pear.php.net/manual/en/standards.php)
   * choisir (pour un nouveau projet) et respecter une unique
     convention de nommage pour les constantes, les variables, les
     fonctions, *etc.*, respectueuse de la *convention de codage*
     utilisée pour le projet - voir [https://fr.wikipedia.org/wiki/Convention_de_nommage](https://fr.wikipedia.org/wiki/Convention_de_nommage)
 * Respecter les référentiels en vigueur dans l'administration
   * [Référentiel général d'interopérabilité](http://references.modernisation.gouv.fr/interoperabilite)
   * [Référentiel général d'accessibilité pour les administrations](http://references.modernisation.gouv.fr/rgaa-accessibilite/)
   * [Référentiel général de sécurité](https://www.ssi.gouv.fr/administration/reglementation/confiance-numerique/le-referentiel-general-de-securite-rgs/)
 * Découper et factoriser tant que possible le code en
   paquetages/bibliothèques/modules internes au projet afin de
   maximiser la réutilisation de code mais aussi d'isoler les
   éventuelles sources d'erreur; avoir recours à des dépôts distincts
   facilite ce cloisonnement
 * Documenter, hors du code et des commentaires
     * l'architecture logicielle du projet (*i.e.* découpage en modules
       fonctionnels et/ou avec des privilèges particuliers)
     * les interfaces exposées par chaque module, la nature et le
       format des informations échangées/stockées
     * les processus d'installation, de configuration et de mise en
       production
 * Commenter le code pour les comportements non triviaux comme :
     * les effets de bord sur des paramètres passés par référence à
       une fonction
     * les conditions d'usage qui ne peuvent être assurées par un
       typage approprié et les effets associés en cas de non-respect ;
       par exemple, une fonction qui réalise une division pour
       laquelle la charge incombe à l'appelant de vérifier que le
       dénominateur n'est pas nul sous peine de générer une erreur à
       l'exécution


## Sécurité

 Il est recommandé d'identifier un responsable de la sécurité du
 projet qui sera garant de vérifier le respect des bonnes pratiques
 mises en œuvre durant le développement, et de traiter les éventuels
 incidents de sécurité. Il est également préférable d'avoir recours à
 une adresse électronique dédiée, à destination du responsable identifié au
 moins, pour traiter des incidents de sécurité qui se produiraient ou
 qui seraient découverts par un tiers.

### Développement sécurisé

 * Écrire du code qui respecte des pratiques de sécurité reconnues et
   qui ne fait pas usage de constructions dangereuses dans le langage utilisé
     * [SEI CERT Coding Standards](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards)
     * [PHP The Right Way](http://eilgin.github.io/php-the-right-way/)
     * [Secure Coding Guidelines for Java SE](http://www.oracle.com/technetwork/java/seccodeguide-139067.html)
     * [Importance des langages pour la sécurité](https://www.ssi.gouv.fr/agence/publication/mind-your-languages-nouvel-article-sur-limportance-des-langages-pour-la-securite/)
     * [Sécurité et langage Java](https://www.ssi.gouv.fr/javasec/)
     * [Sécurité et langages fonctionnels](https://www.ssi.gouv.fr/lafosec/)
 * Éliminer tous les messages de *debug* (par compilation
   conditionnelle ou par un contrôle via une variable à l'exécution) et toute
   information inutile pour l'utilisateur dans les messages d'erreur
   (e.g.  trace d'appel Java/PHP/Python) lors de la mise en production
 * Éliminer tout le code mort (*i.e.* code non appelé/non
   atteignable) car il pourrait prêter à confusion et/ou laisser
   penser qu'il est toujours fonctionnel et testé ; ce code, non
   maintenu, pourrait être réintégré à tort par un développeur
 * Restreindre au strict nécessaire les droits/privilèges attribués
   à chaque module/processus (*i.e.* appliquer une politique de *moindre
   privilège*)
 * Les appels à des fonctions d'exécution de commande système (`exec`,
   `system`, *etc*) doivent être proscrits ; si un usage légitime se
   présente:
     * isoler cet appel dans un module/processus disposant
       **uniquement** des privilèges **strictement nécessaires** aux
       commandes exécutées
     * effectuer un contrôle très strict (e.g. par liste blanche), à défaut d'avoir des
       commandes constantes/fixes, de tous les paramètres passés afin
       d'empêcher l'exécution de commandes arbitraires par un
       attaquant
 * Toutes les entrées externes (e.g. de l'utilisateur) doivent être
   filtrées en explicitant uniquement les cas acceptés (filtrage par
   liste blanche) **avant** leur manipulation/stockage

### Données secrètes/sensibles, cryptographie

 * Aucun élément secret (tel qu'un mot de passe ou une clé
   cryptographique) ne doit être stocké dans le code ou dans les
   commentaires; avoir recours à des fichiers de configuration qui ne
   sont pas versionnés (*cf* `.gitignore`)
 * Aucun élément secret ne doit être écrit par le programme en clair dans un fichier (y
   compris un fichier de journalisation) ou dans une base de données,
   toujours préférer une version hachée par une fonction de hachage
   reconnue à l'état de l'art et correctement utilisée (*i.e* salée
   pour chaque entrée)
     * [Référentiel général de sécurité - Annexe B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)
 * Aucun élément secret ne doit transiter en clair sur le réseau
 * Ne pas implémenter soi-même de mécanisme cryptographique mais
   utiliser des bibliothèques reconnues en utilisant des paramètres
   et des suites cryptographiques robustes
     * [Recommandations de sécurité relatives à TLS](https://www.ssi.gouv.fr/nt-tls/)
     * [Référentiel général de sécurité - Annexe B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)


### Outils de développement et dépendances

 * Utiliser, le cas échéant, des logiciels et des bibliothèques
   tierces maintenus et à jour des correctifs sécurité; préférer des
   bibliothèques (re)connues, et les plus simples possibles
 * Utiliser les services d'analyse de code offerts par la plateforme
   d'hébergement et traiter systématiquement avant intégration les
   problèmes remontés
 * Ne pousser que des *commits* de code qui compilent, testés et
   fonctionnels, accompagnés des tests unitaires correspondants ;
   certaines plateformes offrent la possibilité de rejouer
   automatiquement les tests unitaires d'un projet afin d'assurer la
   non-régression (e.g [Travis](https://docs.travis-ci.com/),
   [Homu](https://github.com/servo/homu))
 * Créer un *tag* (e.g. v2.0.1) pour chaque version (e.g. 2.0.1), et
   le signer cryptographiquement (voir [GPG signature
   verification](https://github.com/blog/2144-gpg-signature-verification))
 * Respecter les recommandations et bonnes pratiques de sécurité émises
   par l'ANSSI applicables au projet
     * [Bonnes pratiques de l'ANSSI](https://www.ssi.gouv.fr/administration/bonnes-pratiques/)
     * [Guide de sécurité méthodologie agile ANSSI / DINSIC](https://www.ssi.gouv.fr/uploads/2017/07/guide-securite-agile_v0.42_anssi_dinsic.pdf)



## Outillage

La politique de contribution n'a pas vocation à proposer un outillage particulier. Toutefois spécifiquement pour la gestion
de code ouvert, vous pourrez trouver les outils référencés sur https://www.linuxfoundation.org/tools-managing-open-source-programs/#1 utiles.
