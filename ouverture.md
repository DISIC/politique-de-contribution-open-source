---
title: Principes d’ouverture des codes sources
menu: 
  main:
    name: "Ouverture"
    weight: 20 
---

## Préambule

### Principe de subsidiarité

La politique peut être instanciée localement avec une priorité plus forte.

Voir la section [instanciation](Instanciation.md) si vous souhaitez décliner cette politique au sein de votre organisation.

### Assistance sur la politique de contribution

Contacter `opensource@data.gouv.fr` pour toute question sur cette politique.

## Principe de reconnaissance des contributions

### Attribuer les contributions aux individus

Afin de reconnaître la paternité des contributions, l'adresse électronique individuelle du développeur est utilisée:

 * Pour les agents : utilisation de l'adresse électronique professionnelle.
 * Pour les prestataires de services, utilisation de l'adresse électronique de leur société d'attachement (pas d'adresse prestataire fournie par l'administration)

Toutefois, au cas où un développeur ne souhaiterait pas voir son identité publiée, il peut utiliser un pseudonyme.  En revanche, l'utilisation d'adresses électroniques génériques ou anonymes est à proscrire.
 
### Distinguer les contributions professionnelles et personnelles

Il est possible pour un développeur de contribuer sur un même projet dans le cadre du milieu professionnel et à titre personnel, l'État reconnaissant aux développeurs la propriété sur les contributions réalisées en dehors du temps de travail. Les contributions réalisées sur le temps professionnel doivent être associées à une adresse électronique professionnelle.

## Contribuer à des projets tiers

### Autorisation par défaut de contribuer à des projets sous licence FSF ou OSI

Les licences validées par les organismes Free Software Foundation et Open Source Initiative et recensées sur leurs pages respectives :

 * FSF : [https://www.gnu.org/licenses/license-list.fr.html](https://www.gnu.org/licenses/license-list.fr.html) (en excluant les licences non libres présentées comme telles) ;
 * OSI : [https://opensource.org/licenses/alphabetical](https://opensource.org/licenses/alphabetical).

À l'inverse les licences non retenues par ces organismes (comme la *Beerware*) ne rentrent pas dans le cadre de l'autorisation par défaut. Un tableau consolidé des licences validées par l'un ou l'autre organisme est maintenu sur le site [https://spdx.org/licenses/](https://spdx.org/licenses)

### Signature des *Corporate Contributor License Agreement*

La DINSIC prend en charge de signer les accords de contributions spécifiques (Corporate Contributor License Agreement ou CCLA) avec les communautés ou les entreprises qui l'exigent, afin de permettre les contributions des agents à titre professionnel aux projets concernés. Si cela est demandé par l'autre partie, elle maintiendra les listes d'individus couverts par l'accord. Une autre possibilité est que l'accord de CCLA soit un pré-requis à la signature d'un Contributor License Agreement individuel (iCLA). Dans ce cas, la signature d'un CCLA par la DINSIC vaudra pré-autorisation pour la signature d'iCLA.

Si vous souhaitez contribuer à un projet réclamant ce type de formalisme, que ce soit pour signer un CCLA, vous rajouter à la liste des contributeurs autorisés, ou vérifier la possibilité de signer un iCLA, contactez l'adresse d'assistance indiquée plus haut.

Liste des CCLA signés :

 * A ce stade, aucun CCLA n'a encore été signé par la DINSIC.

## Contribuer en publiant un nouveau projet

### La publication du code source ne crée ni obligation ni garantie

* Aucune obligation de support et de prise en compte des demandes des utilisateurs ni plus généralement d'obligation d'animer la communauté.
* Pas de garanties au-delà de ce qui est prévu par la licence.

### Autorisation par défaut de contribuer un nouveau projet avec les licences du décret

L'État n'a pas vocation à être éditeur de logiciels. En dehors des trois exceptions prévues à la loi pour une République numérique pour lesquelles vous pouvez contacter l'adresse électronique de support en cas de question, il n'y a pas d'autorisation préalable à demander auprès de la DINSIC. Pour autant, veuillez vous référer à votre supérieur hiérarchique avant la publication d'un nouveau projet dans le compte de votre organisation.

Pour rappel, les licences à utiliser sont disponibles par décret sur le site : [http://www.data.gouv.fr/fr/licences](http://www.data.gouv.fr/fr/licences).

### Éléments à considérer dans le choix de la licence libre

Pour les cas où l'administration a des raisons de garantir que les modifications apportées par un tiers au logiciel libre qu'elle publie sont accessibles sous les mêmes conditions, elle envisagera une licence à réciprocité.  En particulier, s'il s'agit d'un logiciel qui est à la base d'un service en ligne pour lequel elle souhaite se prémunir de toute réappropriation, elle pourra considérer la licence GNU Affero General Public License.  Dans les autres cas, elle considérera les licences permissives.

Le choix de la licence d'un projet devra également prendre en compte celles des composants Open Source tiers constituant son cadre technique, selon les modalités de leurs relations techniques.

L'écosystème où s'insère le projet pourra aussi aiguiller le choix de la licence, dans la limite de la latitude laissée par les critères précédents.

À noter que les solutions logicielles sont souvent modulaires et que la question de la licence peut se poser à plusieurs niveaux.  Par exemple, pour une solution de site web, les modules de l'interface web pourront être publiés sous une licence différente de celle qui couvre le code source côté serveur.

### Distribution des logiciels sous forme de paquets

Le code source des logiciels est souvent empaqueté de façon à être utilisé dans d'autres projets.  Chaque écosystème utilise son système de distributions de paquets: modules `npm` ou `pypi`, images `docker`, fichiers `deb`, etc.

Il est recommandé de distribuer, en plus du code source des logiciels, les paquets qui facilitent leur réutilisation.

Pour connaître les sites sur lesquels publier vos paquets, contactez le [mainteneur](MAINTAINERS) de cette politique correspondant à votre ministère.  Si vous ne savez pas qui contacter, écrivez à `opensource@data.gouv.fr`.

### Certification de l'origine des contributions (DCO)

Les projets publiés par l'État n'exigent pas de droits spécifiques des contributeurs en dehors de ceux accordés par leurs licences respectives (pas d'utilisation de CLA). En revanche, il est demandé aux contributeurs de signer un Certificat d'origine des contributions (*Developer Certificate of Origin*). Afin de s'insérer dans les standards en usage, il a été choisi d'utiliser une traduction française du texte utilisé pour le noyau Linux et repris par de nombreux autres projets.
