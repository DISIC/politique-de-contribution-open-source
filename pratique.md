---
title: Bonnes pratiques
menu:
  main:
    name: "Bonnes pratiques"
    weight: 40
---

## Système de suivi de version de code source

L'utilisation d'un système de suivi de version distribué tel que Git est recommandée. Les systèmes SVN ou CVS sont déconseillés.

## Aide au choix d'une plateforme Web

En plus du système de suivi de version du code source, une plateforme Web propose une panoplie d'outils collaboratifs associés et vise à mobiliser une communauté de développeurs.  Ces plateformes peuvent être hébergées par un tiers ou par l'administration.

Exemples de plateformes Web hébergées par un tiers :

* GitHub : https://github.com
* GitLab : http://gitlab.com (version entreprise)
* Bitbucket : https://bitbucket.org
* Framagit : http://framagit.org - utilisant [GitLab](https://about.gitlab.com/installation/)
* Adullact : http://gitlab.adullact.net - utilisant [GitLab](https://about.gitlab.com/installation/)
* FSFE : https://git.fsfe.org - utilisant [Gitea](https://gitea.io/)
* FSF : https://git.savannah.gnu.org/cgit/ - utilisant [cgit](https://git.zx2c4.com/cgit/)

Les codes source de github.com et bitbucket.org ne sont pas libres, tout comme certains modules de gitlab.com ; certaines plateformes publient des données anonymisées en open data ; leurs portées géographiques peuvent varier, de même que le nombre de développeurs qui l'utilisent.  La liste est incomplète.

Le choix de créer un compte d'organisation au sein d'une plateforme Web existante relève de l'administration, qui peut également héberger sa propre forge publique.

Le positionnement d'un projet sur une forge doit se faire en fonction du niveau de collaboration attendu et des interfaces avec les dépôts privés et le reste de la plateforme de développement.

## Gestion des comptes personnels et d'organisation

Tous les projets initiés par une administration doivent être publiés dans des dépôts au sein de comptes d'organisation. Les dépôts de comptes personnels ne doivent être utilisés que pour des fourches (*forks*) techniques temporaires ou des développements personnels.

Il est recommandé d'avoir deux propriétaires par dépôt.

Il est recommandé que les noms d'utilisateurs des propriétaires des comptes d'organisation apparaissent publiquement.

## Inventaire des comptes d'organisation

Une liste des inventaires des comptes d'organisation connus à ce jour est disponible dans le fichier [comptes-organismes-publics](comptes-organismes-publics): si vous avez connaissance d'un compte d'organisation d'un organisme public qui n'y figure pas, vous pouvez soumettre une proposition via une _pull request_.

Vous pouvez aussi référencer un compte d'organisation comme un compte gouvernemental dans GitHub :

1. Inscrivez vous si ce n'est pas déjà fait dans la communauté [https://github.com/government/welcome](https://github.com/government/welcome) ;

2. Référencez votre compte d'organisation en l'ajoutant sur la page : [https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml](https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml) conformément à la page [https://government.github.com/community/](https://government.github.com/community/).

## Distinction des contributions personnelles / professionnelles

La distinction entre contributions personnelles et professionnelles se base sur l'adresse électronique associée.  Le contributeur doit donc changer celle-ci en fonction de la situation où il se trouve.  Dans le cas de l'utilisation de `git`, cela peut se faire simplement :

* Pour une contribution professionnelle :
<br>`git config user.email "prenom.nom@ministere.gouv.fr"`

* Pour une contribution personnelle :
<br>`git config user.email "email@perso.fr"`

Pour connaître l'adresse électronique actuellement utilisée :
<br>`git config --get user.email`

Dans les cas où le contributeur ne souhaite pas voir son identité personnelle attachée à sa contribution, une adresse électronique (ou alias) devra être mise à disposition par le ministère pour permettre l'utilisation d'un pseudonyme. Attention certains projets open source peuvent refuser les contributions sous pseudonyme.

## Aide au choix de la licence

Le choix d'une licence est aussi le choix d'une communauté de développeurs et d'un écosystème d'outils associés. Une fois la famille de licence trouvée, c'est avant tout la communauté visée qui détermine le choix.

Les licences recommandées par défaut sont :

  * Permissive : Apache 2.0
  * Avec obligation de réciprocité : GNU GPL v3 (standard, lesser ou affero en fonction)

 > Multilicensing : il est possible de fournir un logiciel sous plusieurs licences simultanément, bien que cela puisse entraîner de la confusion.

## Gestion des versions

Avoir une politique de gestion des versions est recommandé. Le guide de versioning sémantique (https://semver.org/lang/fr/) est un bon exemple à suivre.

## Fichiers présents dans le dépôt

Assurez-vous d'avoir au minimum les fichiers README, CONTRIBUTING et LICENSE.

* AUTHORS : décrit la liste des auteurs du programme.

* CODE\_OF\_CONDUCT : un code de conduite pour réguler la communauté de contributeurs.  Voici quelques exemples :  [https://www.djangoproject.com/conduct/](https://www.djangoproject.com/conduct/), [https://github.com/18F/code-of-conduct](https://github.com/18F/code-of-conduct), [Contributor Covenant](https://www.contributor-covenant.org/), [Charte de GNU pour une communication bienveillante](https://www.gnu.org/philosophy/kind-communication.fr.html), etc.

* CONTRIBUTING : guide de contribution, comment s'impliquer et identification du processus de contribution et des licences associées. Exemple: [https://github.com/moby/moby/blob/master/CONTRIBUTING.md](https://github.com/moby/moby/blob/master/CONTRIBUTING.md)

* GOVERNANCE : décrit la gouvernance du projet, les rôles et les droits de votes. Un exemple est disponible dans ce dépôt [gouvernance.md](gouvernance.md).

* INSTALL : description de la procédure d'installation d'un logiciel.

* LICENSE : licence de publication du logiciel.

* MAINTAINERS : liste des mainteneurs du projet (avec des droits de vote ou de commit généralement). Exemple: [https://github.com/moby/moby/blob/master/MAINTAINERS](https://github.com/moby/moby/blob/master/MAINTAINERS)

* NFR : choix d'architecture technique du projet qui ne correspondent pas à des exigences fonctionnelles.

* README : description du projet. Peut décrire l'objectif et l'administration à l'origine de la publication.

* ROADMAP : feuille de route publique.

Ces fichiers doivent être en texte simple ou avec du marquage minimum (ie Markdown). Il n'est pas recommandé d'utiliser des formats binaires (ie PDF).

## Entête des fichiers sources

Conformément aux recommandations détaillées dans [https://reuse.software](https://reuse.software) chaque fichier de code source doit disposer de son auteur, de son identifiant de licence SPDX, ainsi que d'une copie de la licence dans le dépôt local.

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

Ces identifiants permettent de générer automatiquement des inventaires des licences sous la forme de « Bill of Material », afin de garantir la conformité du logiciel.

L'ensemble des identifiants SPDX est disponible à cette adresse : [https://spdx.org/licenses/](https://spdx.org/licenses/)

## Traçabilité des developpements (DCO)

Afin de garantir l'origine des contributions soumises, la mise en œuvre d'un Developer's Certificate of Origin est recommandée.  Une traduction française est mise à disposition [DCO-Fr.txt](https://github.com/DISIC/politique-de-contribution-open-source/blob/master/DCO-fr.txt)

Pour l'instant, le sign-off ne se fait qu'en anglais en utilisant la commande

`git commit --signoff`

## Bonnes pratiques de développement

Les bonnes pratiques de développement courantes s'appliquent également en contexte de développement ouvert, et notamment celles liées au respect des référentiels en vigueur dans l'administration :

* [Référentiel général d'interopérabilité (RGI)](http://references.modernisation.gouv.fr/interoperabilite )
* [Référentiel général d'accessibilité pour les administrations (RGAA)](http://references.modernisation.gouv.fr/rgaa-accessibilite/)
* [Référentiel général de sécurité (RGS)](https://www.ssi.gouv.fr/administration/reglementation/confiance-numerique/le-referentiel-general-de-securite-rgs/)

L'ouverture du code vient par ailleurs amplifier l'importance de certaines de ces bonnes pratiques :

* **Conformité juridique** dans l'utilisation de bibliothèques tierces. La très grande majorité des développements actuels reposant sur des bibliothèques Open Source tierces, il est nécessaire de s'assurer de la compatibilité de leurs licences respectives et du respect des obligations de celles-ci.
* **Modularisation des développements** afin de maximiser la réutilisation de code mais aussi d'isoler les éventuelles sources d'erreur
* **Respect d'une unique convention de développement** par projet.
* **Documentation**, à l'intérieur du code (commentaires et messages de *commit*) et hors du code (voir ci-après).

## Bonnes pratiques de documentation

Les recommandations ci-dessous fixent un idéal, pas un ensemble d'obligations.  Néanmoins, la qualité d'un projet Open Source étant étroitement corrélée à la qualité de sa documentation, on y prêter une attention particulière.

- La documentation est publiée sous [**Licence Ouverte 2.0**][LO link].
- Elle est à jour avec la version du logiciel qu'elle documente.
- Elle propose un manuel utilisateur et un guide du contributeur.
- Elle est lisible en ligne (site web) et hors-ligne (document PDF).
- Elle est rédigée dans un français et/ou un anglais corrects.
- Elle propose plusieurs niveaux d'appropriations (FAQ, tutoriels, manuel approfondi, etc.)
- Elle contient le moins possible de références culturelles ou contextuels risquant de devenir incompréhensibles.

## Sécurité

### Interlocuteur identifié

Il est recommandé d'identifier un responsable de la sécurité du projet qui sera garant de vérifier le respect des bonnes pratiques mises en œuvre durant le développement, et de traiter les éventuels incidents de sécurité. Il est également préférable d'avoir recours à une adresse électronique dédiée, à destination du responsable identifié au moins, pour traiter des incidents de sécurité ou des problèmes liés à la propriété intellectuelle qui seraient découverts par un tiers.

### Développement sécurisé

 * Écrire du code qui respecte des pratiques de sécurité reconnues et qui ne fait pas usage de constructions dangereuses dans le langage utilisé
     * [SEI CERT Coding Standards](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards)
     * [PHP The Right Way](http://eilgin.github.io/php-the-right-way/)
     * [Secure Coding Guidelines for Java SE](http://www.oracle.com/technetwork/java/seccodeguide-139067.html)
     * [Importance des langages pour la sécurité](https://www.ssi.gouv.fr/agence/publication/mind-your-languages-nouvel-article-sur-limportance-des-langages-pour-la-securite/)
     * [Sécurité et langage Java](https://www.ssi.gouv.fr/javasec/)
     * [Sécurité et langages fonctionnels](https://www.ssi.gouv.fr/lafosec/)

* Éliminer tous les messages de *debug* (par compilation conditionnelle ou par un contrôle via une variable à l'exécution) et toute information inutile pour l'utilisateur dans les messages d'erreur (e.g.  trace d'appel Java/PHP/Python) lors de la mise en production

 * Éliminer tout le code mort (*i.e.* code non appelé/non atteignable) car il pourrait prêter à confusion et/ou laisser penser qu'il est toujours fonctionnel et testé ; ce code, non maintenu, pourrait être réintégré à tort par un développeur

 * Toutes les entrées externes (e.g. de l’utilisateur) doivent être contrôlées avant leur utilisation ou leur stockage, selon les bonnes pratiques de sécurité en fonction de leur destination.

### Ne pas compter sur la sécurité par l'obscurité

La sécurité par l'obscurité est globalement reconnue comme une pratique insuffisante, mais dans le cas d'un projet dont le code est ouvert, cette stratégie est caduque. Elle doit donc être remplacée par d'autres stratégies plus robustes comme par exemple la défense en profondeur.

### Données secrètes/sensibles, cryptographie

 * Aucun élément secret (tel qu'un mot de passe ou une clé cryptographique) ne doit être stocké dans le code ou dans les commentaires; avoir recours à des fichiers de configuration qui ne sont pas versionnés (*cf* `.gitignore`)
 * Aucun élément secret ne doit être écrit par le programme en clair dans un fichier (y compris un fichier de journalisation) ou dans une base de données, toujours préférer une version hachée par une fonction de hachage reconnue à l'état de l'art et correctement utilisée (*i.e* salée pour chaque entrée)
     * [Référentiel général de sécurité - Annexe B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)
 * Aucun élément secret ne doit transiter en clair sur le réseau
 * Ne pas implémenter soi-même de mécanisme cryptographique mais utiliser des bibliothèques reconnues en utilisant des paramètres et des suites cryptographiques robustes
     * [Recommandations de sécurité relatives à TLS](https://www.ssi.gouv.fr/nt-tls/)
     * [Référentiel général de sécurité - Annexe B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)


### Outils de développement et dépendances

 * Utiliser, le cas échéant, des logiciels et des bibliothèques tierces maintenus et à jour des correctifs sécurité; préférer des bibliothèques (re)connues, et les plus simples possibles.
 * Utiliser les services d'analyse de code offerts par la plateforme d'hébergement et traiter systématiquement avant intégration les problèmes remontés.
 * Ne pousser que des *commits* de code qui compilent, testés et fonctionnels, accompagnés des tests unitaires correspondants ; certaines plateformes offrent la possibilité de rejouer automatiquement les tests unitaires d'un projet afin d'assurer la non-régression (e.g [Travis](https://docs.travis-ci.com/), [Homu](https://github.com/servo/homu)).
 * Créer un *tag* (e.g. v2.0.1) pour chaque version (e.g. 2.0.1), et le signer cryptographiquement (voir [GPG signature verification](https://github.com/blog/2144-gpg-signature-verification)).
 * Respecter les recommandations et bonnes pratiques de sécurité émises par l'ANSSI applicables au projet
     * [Bonnes pratiques de l'ANSSI](https://www.ssi.gouv.fr/administration/bonnes-pratiques/)
     * [Guide de sécurité méthodologie agile ANSSI / DINSIC](https://www.ssi.gouv.fr/uploads/2017/07/guide-securite-agile_v0.42_anssi_dinsic.pdf)

## Outillage

La politique de contribution n'a pas vocation à proposer un outillage particulier. Toutefois spécifiquement pour la gestion de code ouvert, vous pourrez trouver les outils référencés sur [https://www.linuxfoundation.org/tools-managing-open-source-programs/](https://www.linuxfoundation.org/tools-managing-open-source-programs/#1) utiles.
