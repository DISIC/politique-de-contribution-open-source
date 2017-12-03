+++
title = "Introduction"
weight = 10
[menu.main]
  identifier = "introduction"
+++

# Politique de contribution open-source de l'État

__Historique et versions__

| Version | Commentaire    | Date       |
| --------|----------------|------------|
| 0.1     | Initialisation | 01/11/2017 |

Ce document est en *ALPHA*, ie sous modification intensive sans nécessairement de changement de numéro de version.

## Objectifs

Conformément à la Loi pour une République Numérique du [7 octobre 2016][LoiRepNum link], les codes sources sont des documents 
administratifs communicables et réutilisables. Dans le cas où il est possible de choisir la licence open-source, le décret
[n° 2017-638 du 27 avril 2017][DecretLicences link] précise les familles de licences qui peuvent être utilisées. La liste 
détaillée des licences avec leurs versions est disponible sur le site [data.gouv.fr][Licenses link].

Les objectifs de cette politique de contribution open-source interministérielle sont de :

 * fixer les règles et principes à respecter pour l'ouverture des codes sources
 * accompagner les ministères et partager les meilleures pratiques 
 * définir la gouvernance des politiques de contribution open-source de l'État.

Ce document est à destination des développeurs ou de leurs responsables, qu'ils soient agents publics (titulaires 
ou contractuels) ou prestataires.

## Périmètre

Cette politique de contribution s'applique au système d'information et de communication de l'État 
conformément à l'article 1er du Décret [n° 2014-879 du 1er août 2014][DecretDINSIC link]. Chaque administration de l'État 
a la possibilité d'instancier sa propre politique de contribution pour la préciser et l'amender. 

Sont concernés, l'ensemble des codes sources :

 *  développés en interne par l'administration
 *  développés pour le compte de l'administration.

Cette politique de contribution concerne les *nouveaux* développements afin qu'ils respectent les meilleures pratiques. Pour l'ouverture de codes source existant, des actions complémentaires seront nécessaires, telles que la définition du périmètre d'ouverture du code, sa revue qualité, sa revue sécurité, l'analyse de conformité et l'analyse de la propriété intellectuelle.

Les fonctions publiques hospitalières et territoriales sont hors périmètre de cette politique de contribution, mais elles peuvent s'en inspirer librement.

## Structure du document

La politique de contribution est composée de :

 * [Principes d'ouverture des codes sources](Ouverture.md)
 * [Modalités et meilleures pratiques](Pratique.md)
 * [Instanciation de politique de contribution ministérielle](Instanciation.md)
 * [Gouvernance associée](Gouvernance.md)

Afin d'en faciliter la lecture chaque partie débute par une section TL;DR (Too Long ; Didn't read) qui en résume l'essentiel.

## Responsabilité du document

La DINSIC produit et maintient ce document ; elle veille à sa mise en oeuvre et assure le support associé. Pour toute question, ou demande d'évolutions, veuillez vous référer à la partie *Gouvernance*.

{{< figure
  src="/_assets/images/logo-licence-ouverte-open-licence.png"
  width="300px"
  alt="licence ouverte"
  link="https://github.com/DISIC/politique-de-contribution-open-source/raw/master/LICENSE.pdf"
>}}

Ce document est publié sous la [**Licence Ouverte 2.0**][LO link]

## Références externes

Ce document a été élaborés grâce aux nombreux travaux ci-dessous :

 * Open Government Partnership collaboration : [https://github.com/DISIC/foss-contrib-policy-template](https://github.com/DISIC/foss-contrib-policy-template)
 * USA 18F: [https://github.com/18F/open-source-policy/blob/master/CONTRIBUTING.md](https://github.com/18F/open-source-policy/blob/master/CONTRIBUTING.md)
 * Whitehouse source code policy: [https://sourcecode.cio.gov](https://sourcecode.cio.gov)
 * UK GDS : [http://gds-operations.github.io/guidelines/](http://gds-operations.github.io/guidelines/)
 * Canada British Columbia : [https://github.com/bcgov/BC-Policy-Framework-For-GitHub](https://github.com/bcgov/BC-Policy-Framework-For-GitHub)
 * Linux Foundation open-source guides: [https://www.linuxfoundation.org/resources/open-source-guides/](https://www.linuxfoundation.org/resources/open-source-guides/)
 * Core Infrastructure Initiative: [https://bestpractices.coreinfrastructure.org/](https://bestpractices.coreinfrastructure.org/)
 * Open-Source Guide: [https://opensource.guide/](https://opensource.guide/)
 * FSFE software reuse: [https://reuse.software/](https://reuse.software/)
 * Google open-source: [http://opensource.google.com](http://opensource.google.com)

Un travail est également en cours par le gouvernement du Canada : [https://github.com/canada-ca/Open_First_Whitepaper](https://github.com/canada-ca/Open_First_Whitepaper)

[Logo LO]: https://www.etalab.gouv.fr/wp-content/uploads/2011/10/licence-ouverte-open-licence.gif
[LO link]: https://github.com/DISIC/politique-de-contribution-open-source/raw/master/LICENSE.pdf
[LoiRepNum link]: https://www.legifrance.gouv.fr/affichTexte.do;jsessionid=6E9C9BD1F4AAF6E6FD525E8FE902A615.tplgfr26s_2?cidTexte=JORFTEXT000033202746&categorieLien=id
[DecretDINSIC link]:  https://www.legifrance.gouv.fr/affichTexte.do;jsessionid=6E9C9BD1F4AAF6E6FD525E8FE902A615.tplgfr26s_2?cidTexte=JORFTEXT000029337021&idArticle=&dateTexte=20171101
[DecretLicences link]: https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000034502557&categorieLien=id
[Licenses link]: https://www.data.gouv.fr/fr/licences
