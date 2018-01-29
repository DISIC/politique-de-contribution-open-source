---
title: Gouvernance de la politique de contribution interministérielle
weight: 50
menuName: gouvernance
---

## Parties prenantes 

La DINSIC maintient ce document et en est responsable (elle est propriétaire du dépôt pour la gestion des droits d'écriture) mais l'élaboration de celui-ci a vocation à être collaborative et les entités auxquelles il s'applique sont toutes invitées à participer à son évolution.

Deux types d'organisations sont distinguées :

* Interministériel : DINSIC et ANSSI
* Ministère

avec un seul rôle par organisation (droit d'écriture sur cette politique). L'ensemble des contributeurs avec les droits d'écriture sont listés dans le fichier [MAINTAINERS](MAINTAINERS).


## Gestion des contributions et maintenance

Toutes les contributions sont les bienvenues.  Elles sont faites via une *pull request* sur la branche `next`.

Les `pull request` apportant des modifications **mineures** peuvent ensuite être fusionnées sur la branche `master` par l'un des mainteneurs.

Les `pull request` apportant des modifications **majeures** doivent au préalable être approuvées par au moins trois mainteneurs via le système de vote des issues github.

## Gestion des versions

La politique de contribution open source peut être modifiée pour des changements légers (coquilles, etc.) sans mise à jour de version.

Des compléments et ajustements peuvent être effectués avec une mise à jour du MINEUR du numéro de version directement par la DINSIC et la revue d'un ministère.

Des modifications de règles ou ajouts de règles substantielles nécessitent l'accord de la DINSIC et de 3 ministères au moins pour être validées avec une mise à jour du MAJEUR du numéro de version.

Chaque mise à jour de la version, mineure ou majeure, entraîne l'ajout d'un tag sur le commit correspondant.  Par exemple, la version `0.3` est taggée `v0.3` suivant le schéma `v[MAJEUR].[MINEUR]`.

Toutes les modifications peuvent être faites au fil de l'eau. Les discussions et commentaires sont tracées dans les commentaires de la *pull request*.
