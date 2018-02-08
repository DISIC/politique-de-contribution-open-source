---
title: Principes d’ouverture des codes sources
weight: 20 
menuName: ouverture
---

## Préambule

### Principe de subsidiarité

La politique peut être instanciée localement avec une priorité plus forte.

Voir la section [instanciation](Instanciation.md) si vous souhaitez décliner cette politique au sein de votre organisation.

### Assistance sur la politique de contribution

Contacter `opensource @ data.gouv.fr` pour toute question sur cette politique.

## Principe de reconnaissance des contributions

### Attribuer les contributions aux individus

Reconnaissance individuelle des développeurs : utilisation de leur adresse électronique pour tracer leurs contributions.

 * Pour les agents : utilisation de l'adresse électronique professionnelle.
 * Pour les prestataires de services, utilisation de l'adresse électronique de leur société d'attachement (pas d'adresse prestataire fournie par l'administration)

Possibilité d'utiliser des pseudonymes.

Pas d'utilisation d'adresses électroniques génériques ou anonymes.
 
### Distinguer les contributions professionnelles et personnelles

Possibilité de contribuer sur un même projet dans le cadre du milieu professionnel ou à titre personnel. L'adresse électronique professionnelle doit être utilisée sur le temps professionnel.

## Contribuer à des projets tiers

### Autorisation par défaut de contribuer à des projets sous licence FSF ou OSI

Les licences validées par les organismes Free Software Foundation et Open Source Initiative et recensées sur leurs pages respectives :

 * FSF : https://www.gnu.org/licenses/license-list.fr.html (en excluant les licences non libres présentées comme telles) ;
 * OSI : https://opensource.org/licenses/alphabetical.

À l'inverse les licences non retenues par ces organismes (comme la *Beerware*) ne rentrent pas dans le cadre de l'autorisation par défaut. Un tableau consolidé des licences validées par l'un ou l'autre organisme est maintenu sur le site [https://spdx.org/licenses/](https://spdx.org/licenses)

### Signature des *Corporate Contributor License Agreement*

La DINSIC se charge de signer les accords de contributions spécifiques et de tenir à jour les listes d'individus couverts par ceux-ci.
Si vous souhaitez contribuer à un projet réclamant ce type de formalisme, contactez l'adresse d'assistance indiquée plus haut.

## Contribuer en publiant un nouveau projet

### La publication du code source ne crée ni obligation ni garantie

* Aucune obligation de support et de prise en compte des demandes des utilisateurs ni plus généralement d'obligation d'animer la communauté. 
* Pas de garanties au-delà de ce qui est prévu par la licence.

### Autorisation par défaut de contribuer un nouveau projet avec les licences du décret

L'État n'a pas vocation à être éditeur de logiciels. En dehors des trois exceptions prévues à la loi pour une République numérique pour lesquelles vous pouvez contacter l'adresse électronique de support en cas de question, il n'y a pas d'autorisation préalable à demander auprès de la DINSIC. Pour autant, veuillez vous référer à votre supérieur hiérarchique avant la publication d'un nouveau projet dans le compte de votre organisation.

Pour rappel, les licences à utiliser sont disponibles par décret sur le site : http://www.data.gouv.fr/fr/licences.

### Éléments à considérer dans le choix de la licence libre

Pour les cas où l'administration a des raisons de garantir que les modifications apportées par un tiers au logiciel libre qu'elle publie sont accessibles sous les mêmes conditions, elle envisagera une licence à réciprocité.  En particulier, s'il s'agit d'un logiciel qui est à la base d'un service en ligne pour lequel elle souhaite se prémunir de toute réappropriation, elle pourra considérer la licence GNU Affero General Public License.  Dans les autres cas, elle considérera les licences permissives.

Le choix de la licence d'un projet devra également prendre en compte celles des composants Open Source tiers constituant son cadre technique, selon les modalités de leurs relations techniques.

L'écosystème où s'insère le projet pourra aussi aiguiller le choix de la licence, dans la limite de la latitude laissée par les critères précédents.

À noter que les solutions logicielles sont souvent modulaires et que la question de la licence peut se poser à plusieurs niveaux.  Par exemple, pour une solution de site web, les modules de l'interface web pourront être publiés sous une licence différente de celle qui couvre le code source côté serveur.

### Certification de l'origine des contributions (DCO)

Les projets publiés par l'État n'exigent pas de droits spécifiques des contributeurs en dehors de ceux accordés par leurs licences respectives (pas d'utilisation de CLA). En revanche, il est demandé aux contributeurs de signer un Certificat d'origine des contributions (*Developer Certificate of Origin*). Afin de s'insérer dans les standards en usage, il a été choisi d'utiliser une traduction française du texte utilisé pour le noyau Linux et repris par de nombreux autres projets.
