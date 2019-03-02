---
title: Governance of the Interdepartmental Contribution Policy
menu: 
  main:
    name: "Governance"
    weight: 50
---

The DINSIC maintains this document and is responsible for it (it owns the repository and manages the permissions). The development of this policy aims to be collaborative and the entities to which it applies are all invited to participate in its development.

Two types of organizations are distinguished:

* Interdepartmental: DINSIC and ANSSI
* Ministry

with only one role per organization (write permission on this policy). All contributors with write permissions are listed in the [MAINTAINERS](https://github.com/DISIC/politique-de-contribution-open-source/blob/master/MAINTAINERS) file.

## Management of contributions

All contributions are welcome. They are made via a *pull request* on the branch `next` which is the branch of the next version of the policy.

* pull request with **major** changes must be approved by at least three ministerial organizations and the ANSSI.

* pull requests with **minor** changes must be approved by at least one departmental organization.
 
All maintainers have the ability to merge *pull requests* on the `next` branch. If several maintainers belong to the same department, their validation only counts for one organization.

## Version Management

Only the DINSIC and the ANSSI can merge to the `master` branch which corresponds to the validated version:

* At each merge on the `master` branch a tag is added according to the` v [MAJOR] v. [MINOR] `scheme according to the approved *pull requests* on the` next` branch.

* The open source contribution policy can be modified for slight changes (typos, etc.) without updating the version (semver PATCH numbers are ignored) directly on the `master` branch.

All modifications can be done at any given time. Discussions and comments are logged in the comments of the *pull request*.
