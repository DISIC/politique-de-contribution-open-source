---
title: Principes d'ouverture des codes sources
weight: 20 
menuName: ouverture
---

## En résumé

 * Principe de subsidiarité : la politique peut être instanciée localement avec une priorité plus forte
 * Reconnaissance individuelle des développeurs
 * Distinction des contributions professionnelles / personnelles
 * Pas d'engagements (ni support / ni revue des suggestions de modification)
 * Autorisation par défaut de contribuer aux projets sous license FSF ou OSI
 * Autorisation par défaut de contribuer un nouveau projet avec les licences du décret
 * Recommandation d'utiliser les familles de licences permissives dans le cas général
 * Autorisation par défaut de signer un iCLA (individual CLA) avec les organismes pour lesquels la DINSIC a signé un global CLA
 * Utilisation des DCO (developper's certificate of origin) et ne pas exiger des CLA
 * Support : Contacter `opensource @ data.gouv.fr` pour toute question

## Subsidiarité

Voir la section [instanciation](Instanciation.md) si vous souhaitez décliner cette politique au sein de votre organisation.

## Reconnaissance individuelle

Reconnaissance individuelle des développeurs :  utilisation de leur adresse email pour tracer leurs contributions.

 * Pour les agents : utilisation du mail professionnel en .gouv.fr
 * Pour les prestataires de services, utilisation du mail de leur société d'attachement (pas de mail prestataire en .gouv.fr)

Possibilité d'utiliser des pseudonymes.

Pas d'utilisation de mails génériques / anonymes.
 
## Distinction des contributions professionnelles / personnelles

Possibilité de contribuer sur un même projet dans le cadre du milieu professionnel ou à titre personnel. Le mail professionnel doit être utilisé sur le temps professionnel.

## Pas d'engagements

* Aucune obligation de support et de prise en compte des demandes des utilisateurs ni plus généralement d'obligation d'animer la communauté. 
* Pas de garanties au-delà de ce qui est prévu par la licence.

## Autorisation par défaut de contribuer à des projets sous license FSF ou OSI

Les licences validées par les organismes Free Software Foundation et Open Source Initiative et recensées sur leurs pages respectives :

 * FSF : https://www.gnu.org/licenses/license-list.fr.html (en excluant les licences non libres présentées comme telles) ;
 * OSI : https://opensource.org/licenses/alphabetical.

À l'inverse les licenses de type WTFL ou beerware ne rentrent pas dans le cadre de l'autorisation par défaut (et ne devraient pas être utilisées).

## Autorisation par défaut de contribuer à un nouveau projet avec les licences du décret

L'État n'a pas vocation à être éditeur logiciel. En dehors des trois exceptions prévues à la loi pour une République numérique pour lesquelles vous pouvez contacter le mail de support en cas de question, il n'y a pas d'autorisation préalable à demander auprès de la DINSIC. Pour autant, veuillez vous référer à votre supérieur hiérarchique avant la publication d'un nouveau projet dans le compte de votre organisation.

Pour rappel, les licences à utiliser sont disponibles par décret sur le site : http://www.data.gouv.fr/fr/licences.

## Recommandation d'utiliser des licences permissives dans le cas général

Par défaut, les licences de la famille permissives sont privilégiées par l'administration afin de faciliter la diffusion des codes sources et leur réutilisation en limitant les risques d'incompatibilités avec les licences préexistantes. Ces licences seront particulièrement adaptées pour couvrir les codes sources implémentant un service de base ou d’infrastructure qui a vocation à être inclus dans d’autres services ou appelé par d’autres services (bibliothèques, frameworks...).

Cependant, le choix d’une licence de partage à l’identique peut être pertinent dans les cas suivants pour prévenir toute appropriation propriétaire :

 *	Service d’intérêt général.
 *	Service « contributif » : service en ligne dont la valeur est issue des contributions des utilisateurs du service. 
 *	Service qui organise un écosystème. Permet de partager les évolutions avec l’ensemble des acteurs.
 *	Service décentralisé qui est instancié de nombreuses fois et dont les instances doivent communiquer entre elles.
 *	Service qui établit un lien fort avec le citoyen qui doit être préservé sans que d’autres services puissent l’encapsuler.

À noter que les licences de partage à l’identique sont plus complexes, notamment sur leur clause de distribution (lien statique/dynamique, accès distant, etc.)

## Pré-autorisation de signer un iCLA auprès de certaines communautés

À ce stade aucun corporate CLA n'a été signé avec des communautés. La DINSIC prendra contact et établira les communautés prioritaires avec qui ces contributions seront facilitées.

## Assistance sur la politique de contribution

Contacter `opensource @ data.gouv.fr` pour toute question sur cette politique.
