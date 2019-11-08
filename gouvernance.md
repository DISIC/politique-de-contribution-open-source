---
title: Gouvernance de la politique de contribution interministérielle
menu: 
  main:
    name: "Gouvernance"
    weight: 50
---

La DINSIC maintient ce document et en est responsable (elle est propriétaire du dépôt et de la gestion des droits d'écriture). L'élaboration de cette politique a vocation à être collaborative et les entités auxquelles elle s'applique sont toutes invitées à participer à son évolution.

Deux types d'organisations sont distinguées :

* Interministériel : DINSIC et ANSSI
* Ministériel

avec un seul rôle par organisation (droit d'écriture sur cette politique). L'ensemble des contributeurs avec les droits d'écriture sont listés dans le fichier [MAINTAINERS](https://github.com/DISIC/politique-de-contribution-open-source/blob/master/MAINTAINERS).

## Gestion des contributions

Toutes les contributions sont les bienvenues.  Elles sont faites via une *pull request* sur la branche `next` qui est la branche d'élaboration d'une nouvelle version de la politique.

 * les `pull request` apportant des modifications **majeures** doivent être approuvées par au moins trois autres organisations ministérielles et l'ANSSI.

 * les `pull request` apportant des modifications **mineures** doivent être approuvées par au moins une autre organisation ministérielle.
 
Tous les mainteneurs ont la possibilité de fusionner les *pull requests* sur la branche `next`. Si plusieurs mainteneurs appartiennent à un même ministère, leur validation ne compte que pour une organisation.

## Gestion des versions

Seules la DINSIC et l'ANSSI peuvent fusionner sur la branche `master` qui correspond à la version validée :

 * À chaque fusion sur la branche `master` un tag est ajouté suivant le schéma `v[MAJEUR].[MINEUR]` en fonction des *pull requests* approuvées sur la branche `next`. 

 * La politique de contribution open source peut être modifiée pour des changements légers (coquilles, etc.) sans mise à jour version (les numéros de PATCH de semver sont ignorés) directement sur la branche `master`.

Toutes les modifications peuvent être faites au fil de l'eau. Les discussions et commentaires sont tracées dans les commentaires de la *pull request*.
