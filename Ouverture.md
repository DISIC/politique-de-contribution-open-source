---
title: Ouverture
---

## Principes d'ouverture des codes sources

### TL:DR

 * Principe de subsidiarité : la politique peut être instanciée localement avec une priorité plus forte
 * Reconnaissance individuelle des développeurs
 * Distinction des contributions professionnelles / personnelles
 * Pas d'engagements (ni support / ni suggestions de modification)
 * Autorisation par défaut de contribuer aux projets sous licenses FSF ou OSI
 * Autorisation par défaut de contribuer un nouveau projet avec les licences du décret
 * Recommandation d'utiliser les familles de licences permissives dans le cas général
 * Autorisation par défaut de signer un iCLA (individual CLA) avec les organismes pour lesquels la DINSIC a signé un global CLA
 * Utilisation nécessaire d'un système de suivi de version distribué (git, bitbucket, mercurial) et possibilité d'utiliser toute plateforme (github, gitlab, framagit, ...)
 * Vérification en termes de sécurité de la non-divulgation de secrets ou données personnnelles
 * Inventaire des comptes d'organisation gouvernementaux
 * Utilisation possible des DCO (developper's certificate of origin) et ne pas exiger des CLA
 * Support: Contacter `opensource @ data.gouv.fr` pour toute question

### Subsidiarité

Voir instanciation si vous souhaitez décliner cette politique au sein de votre organisation

### Reconnaissance individuelle

Reconnaissance individuelle des développeurs :  Utilisation de leur adresses emails pour tracer leurs contributions.

 * Pour les agents: utilisation du mail professionnel en .gouv.fr
 * Pour les prestataires de services, utilisation du mail de leur société d'attachement (pas de mail prestataire en .gouv.fr)

Possibilité d'utiliser des pseudonymes.

Pas d'utilisation de mails génériques / anonymes
 
### Distinction des contributions professionnelles / personnelles

Possibilité de contribuer sur un même projet dans le cadre du milieu professionnel ou à titre personnel. Le mail professionnel doit être utilisé sur le temps professionnel.

### Pas d'engagements

Aucune obligation d'étudier les pull requests transmises. Pas de support ni de garantie conformément aux licenses.

### Autorisation par défaut de contribuer à des projets sous licenses FSF ou OSI

Les licences validées par les organismes Free Software Foundation et Open Source Initiative et recensées sur leurs pages respectives :

 * FSF : https://www.gnu.org/licenses/license-list.fr.html 
 * OSI : https://opensource.org/licenses/alphabetical

A l'inverse les licenses de type WTFL ou beerware ne rentrent pas dans le cadre de l'autorisation par défaut.

### Autorisation par défaut de contribuer un nouveau projet avec les licences du décret

L'Etat n'a pas vocation à être éditeur logiciel. En dehors des trois exceptions prévues à la loi république numérique pour lesquelles vous pouvez contacter le mail de support en cas de question, il n'y a pas d'autorisation préalable à demander auprès de la DINSIC. Pour autant veuillez vous référer à votre manager direct avant la publication d'un nouveau projet dans le compte de votre organisation.

Pour rappel, les licences à utiliser sont disponibles par décret sur le site : http://www.data.gouv.fr/fr/licences

### Recommandation d'utiliser des licences permissives dans le cas général

Pour l’administration, par défaut, les licences de la famille permissives sont privilégiées afin de ne pas introduire de biais de concurrence et empêcher un acteur (commercial et propriétaire) de bénéficier du code développé par l’administration. Ainsi de nouveaux services à valeur ajoutée peuvent être développés par des acteurs tiers, même si ces derniers restent propriétaires (et payants).

Toutefois, le choix d’une licence de partage à l’identique peut être pertinent dans les cas suivants pour prévenir toute appropriation propriétaire :

 *	Service d’intérêt général
 *	Service « contributif » : service en ligne dont la valeur est issue des contributions des utilisateurs du service. 
 *	Service qui organise un écosystème. Permet de partager les évolutions avec l’ensemble des acteurs.
 *	Service décentralisé qui est instancié de nombreuses fois et dont les instances doivent communiquer entre elles.
 *	Service qui établit un lien fort avec le citoyen qui doit être préservé sans que d’autres services puissent l’encapsuler

A noter que les licences de partage à l’identique sont plus complexes notamment sur leur clause de distribution (lien statique/dynamique, accès distant, etc.)

A l’inverse, si c’est un service de base ou d’infrastructure qui a vocation à être inclus dans d’autres services ou appelé par d’autres services, la balance penche plutôt pour des licences permissives.

### Pré-autorisation de signer un iCLA auprès de certaines communautés

A ce stade aucun corporate CLA n'a été signé avec des communautés. La DINSIC prendra contact et établira les communautés prioritaires avec qui ces contributions seront facilitées.

### Assistance sur la politique de contribution

Contacter `opensource @ data.gouv.fr` pour toute question sur cette politique
