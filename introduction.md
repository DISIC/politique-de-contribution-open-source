---
title: Politique de contribution aux logiciels libres de l’État
weight: 10
menuName: introduction
---

__Historique et versions__

| Version | Commentaire                                     | Date       |
| --------|-------------------------------------------------|------------|
| 0.1     | Initialisation                                  | 01/11/2017 |
| 0.2     | Ouverture de l'appel à commentaires             | 06/12/2017 |
| 0.3     | Fin de l'appel à commentaires                   | 28/01/2018 |

Ce document est en *ALPHA*, ie sous modification intensive sans nécessairement de changement de numéro de version.

## Objectifs

Conformément à la Loi pour une République numérique du [7 octobre 2016][LoiRepNum link], les codes sources sont des documents 
administratifs communicables et réutilisables. Dans le cas où il est possible de choisir une licence libre, le décret
[n° 2017-638 du 27 avril 2017][DecretLicences link] précise les familles de licences qui peuvent être utilisées. La liste 
détaillée des licences avec leurs versions est disponible sur le site [data.gouv.fr][Licenses link].

Les objectifs de cette politique interministérielle de contribution aux logiciels libres sont de :

 * fixer les règles et principes à respecter pour l'ouverture des codes sources
 * accompagner les ministères et partager les bonnes pratiques 
 * définir la gouvernance des politiques de contribution de l'État.

Ce document est à destination des développeurs ou de leurs responsables, qu'ils soient agents publics (titulaires 
ou contractuels) ou prestataires.

## Périmètre

Cette politique de contribution s'applique au système d'information et de communication de l'État 
conformément à l'article 1er du [décret n° 2014-879 du 1er août 2014][DecretDINSIC link]. Chaque administration de l'État 
a la possibilité d'instancier sa propre politique de contribution pour la préciser et l'amender. 

Sont concernés l'ensemble des codes sources :

 *  développés en interne par l'administration
 *  développés pour le compte de l'administration.

Cette politique de contribution vise les *nouveaux* développements afin qu'ils respectent les bonnes pratiques. Pour l'ouverture de codes sources existants, des actions complémentaires seront nécessaires, telles que la définition du périmètre d'ouverture du code, sa revue qualité, sa revue sécurité, l'analyse de conformité et l'analyse de la propriété intellectuelle.

Les fonctions publiques hospitalières et territoriales sont hors périmètre de cette politique de contribution mais elles peuvent s'en inspirer librement.

## Structure du document

La politique de contribution est composée de :

 * [Principes d’ouverture des codes sources]({{< relref "ouverture.md" >}} )
 * [Modalités et bonnes pratiques]({{< relref "pratique.md" >}})
 * [Instanciation de politique de contribution ministérielle]({{< relref "instanciation.md" >}})
 * [Gouvernance associée]({{< relref "gouvernance.md" >}})

## Responsabilité du document

La DINSIC produit et maintient ce document ; elle veille à sa mise en œuvre et assure le support associé. Pour toute question, ou demande d'évolutions, veuillez vous référer à la partie *Gouvernance*.

Ce document est publié sous la [**Licence Ouverte 2.0**][LO link]

## Références externes

Ce document a été élaboré grâce aux nombreux travaux ci-dessous :

 * Open Government Partnership collaboration : 
 <br>[https://github.com/DISIC/foss-contrib-policy-template](https://github.com/DISIC/foss-contrib-policy-template)
 * USA 18F Open Source Policy : 
 <br>[https://github.com/18F/open-source-policy/blob/master/CONTRIBUTING.md](https://github.com/18F/open-source-policy/blob/master/CONTRIBUTING.md)
 * Whitehouse Source Code Policy : 
 <br>[https://sourcecode.cio.gov](https://sourcecode.cio.gov)
 * UK GDS (Governement Digital Service) : 
 <br>[http://gds-operations.github.io/guidelines/](http://gds-operations.github.io/guidelines/)
 * Canada British Columbia : 
 <br>[https://github.com/bcgov/BC-Policy-Framework-For-GitHub](https://github.com/bcgov/BC-Policy-Framework-For-GitHub)
 * Australia Digital Transformation Agency : 
 <br>[https://www.dta.gov.au/standard/8-make-source-code-open/](https://www.dta.gov.au/standard/8-make-source-code-open/)
 * Linux Foundation Open Source Guides : 
 <br>[https://www.linuxfoundation.org/resources/open-source-guides/](https://www.linuxfoundation.org/resources/open-source-guides/)
 * Core Infrastructure Initiative : 
 <br>[https://bestpractices.coreinfrastructure.org/](https://bestpractices.coreinfrastructure.org/)
 * Open Source Guides : 
 <br>[https://opensource.guide/](https://opensource.guide/)
 * FSFE software reuse : 
 <br>[https://reuse.software/](https://reuse.software/)
 * Google Open Source : 
 <br>[http://opensource.google.com](http://opensource.google.com)

Un travail est également en cours par le gouvernement du Canada : [https://github.com/canada-ca/Open_First_Whitepaper](https://github.com/canada-ca/Open_First_Whitepaper)

[Logo LO]: https://www.etalab.gouv.fr/wp-content/uploads/2011/10/licence-ouverte-open-licence.gif
[LO link]: https://github.com/DISIC/politique-de-contribution-open-source/raw/master/LICENSE.pdf
[LoiRepNum link]: https://www.legifrance.gouv.fr/affichTexte.do;jsessionid=6E9C9BD1F4AAF6E6FD525E8FE902A615.tplgfr26s_2?cidTexte=JORFTEXT000033202746&categorieLien=id
[DecretDINSIC link]:  https://www.legifrance.gouv.fr/affichTexte.do;jsessionid=6E9C9BD1F4AAF6E6FD525E8FE902A615.tplgfr26s_2?cidTexte=JORFTEXT000029337021&idArticle=&dateTexte=20171101
[DecretLicences link]: https://www.legifrance.gouv.fr/affichTexte.do?cidTexte=JORFTEXT000034502557&categorieLien=id
[Licenses link]: https://www.data.gouv.fr/fr/licences
