---
title: Best practices
menu: 
  main:
    name: "Best practices"
    weight: 30
---

## Source code version tracking system

Using a distributed version tracking system such as git is recommended. Svn or cvs systems are deprecated.

## Help in choosing a web platform

In addition to the source code version tracking system, a web platform offers a range of associated collaborative tools and aims to mobilize a community of developers. These platforms may be hosted by a third party or by the administration.

Examples of web platforms hosted by a third party:

* GitHub: [https://github.com](https://github.com)
* GitLab: [http://gitlab.com](http://gitlab.com) (enterprise version)
* Bitbucket : https://bitbucket.org
* Adullact: [http://gitlab.adullact.net](http://gitlab.adullact.net) - using [GitLab](https://about.gitlab.com/installation/)
* FSFE: [https://git.fsfe.org](https://git.fsfe.org) - using [Gitea](https://gitea.io/)
* FSF: [https://git.savannah.gnu.org/cgit/](https://git.savannah.gnu.org/cgit/) - using [cgit](https://git.zx2c4.com/cgit/)

The source code of github.com is not free just like some modules of gitlab.com; some platforms publish anonymous data in open data; their geographic scope may vary, as well as the number of developers who use it. The list is incomplete.

The choice to create an organizational account within an existing Web platform is the responsibility of the administration, which can also host its own public forge.

Choosing a forge for a project must be done according to the level of collaboration expected and the interfaces with the private repositories and the rest of the development platform.

To know on which forge you should publish your source code, contact the [maintaineur](MAINTAINERS) of this policy from your ministry. If you don't know who you should get in touch with, send an email to `opensource@data.gouv.fr`.

## Management of personal and organizations accounts

All projects initiated by an administration must be published in repositories under an organization accounts. Personal account repositories should only be used for temporary technical forks or personal developments.

Here are the recommendations for managing organization accounts or groups:

- make the users and owners publicly visible;
- publish at least one email address as the contact email;
- indicate what website is associated with the organization account;
- if the platform allows it, verified the website associated with the account;
- add a description and a picture.

To handle repositories, it is recommended to have at least two organization owners and to publish the email address of at least one owner.

## Inventory of organization accounts

A list of known forges and organization accounts from the public sector is readable in the [comptes-organismes-publics](comptes-organismes-publics) file : if you happen to know a forge or an organization account that should appear in this list, please submit a _pull request_.

This list is used for [code.etalab.gouv.fr](https://code.etalab.gouv.fr) which allows anyone to look for repositories within all forges and organization accounts.

You can also reference an organization account as a government account in GitHub:

1. Register if you have not done so already in the community [https://github.com/government/welcome](https://github.com/government/welcome)

2. Reference your organization account by adding it on the page: [https://github.com/github/government.github.com/blob/gh-pages/_data/governments.yml](https:// github.com/github/government.github.com/blob/gh-pages/_data/governments.yml) as per [https://government.github.com/community/](https://government.github .com / community /)

## Distinction of personal / professional contributions

The distinction between personal and professional contributions is based on the associated email address.  The contributor must change its email accordingly.

In the case of using `git`, this can be done easily:

* For a professional contribution:

`git config user.email "firstname.lastname@ministere.gouv.fr"`

* For a personal contribution:

`git config user.email "email@perso.fr"`

To find the email address currently used:

`git config --get user.email`

In cases where the contributor does not wish to see his personal identity attached to his contribution, an email address (or alias) need to be made available by the department to allow the use of a pseudonym. Beware some open source projects may refuse contributions under pseudonym.

## Help in choosing the license

The choice of a license is also the choice of a community of developers and an ecosystem of associated tools. Once the license family is chosen, it is primarily the targeted developer's community that determines the choice.

The recommended licenses by default are:

* Permissive: Apache 2.0
* Reciprocal: GNU GPL v3 (standard, lesser or affero in function)

> Multilicensing: It is possible to provide software under several licenses simultaneously, although this can lead to confusion.

## Version Management

Having a versioning policy is recommended. The semantic versioning guide (https://semver.org/lang/en/) is a good example to follow.

## Files in the repository

Make sure you have at least the README, CONTRIBUTING, and LICENSE files.

* CODE\_OF\_CONDUCT : a code of conduct to regulate the community of contributors. Examples can be found: [https://www.djangoproject.com/conduct/](https://www.djangoproject.com/conduct/) and [https://github.com/18F/code-of- conduct](https://github.com/18F/code-of-conduct).

* CONTRIBUTING: contribution guide, how to get involved and identification of the contribution process and associated licenses. Example: [https://github.com/moby/moby/blob/master/CONTRIBUTING.md](https://github.com/moby/moby/blob/master/CONTRIBUTING.md)

* GOVERNANCE: describes project governance, roles and voting rights. An example is available in this repository [gouvernance.md](gouvernance.md).

* INSTALL: install instructions.

* LICENSE: software license.

* MAINTAINERS: list of project maintainers (usually with voting or commit rights). Example: [https://github.com/moby/moby/blob/master/MAINTAINERS](https://github.com/moby/moby/blob/master/MAINTAINERS)

* NFR: choice of technical architecture of the project that do not correspond to functional requirements.

* README: description of the project. Can describe the purpose and the administration behind the publication.

* ROADMAP: public road map.

These files must be in plain text or with minimum marking (ie Markdown). It is not recommended to use binary formats (ie PDF).

## Heads source files

According to the detailed recommendations in [https://reuse.software](https://reuse.software) each source code file must have its author, SPDX license ID, and a copy of the license in the local repository.

  * Examples of file header (headers):

```
 / *
  * Copyright (c) 2017 Alice Commit <alice@example.com>
  *
  * SPDX-License-Identifier: BSD-2-Clause
  * License-Filename: LICENSES / BSD-2-Clause_Alice.txt
  * /
```

or in the case of a project that automatically tracks its contributors:

```
 / *
  * This file is part of the project X. It's copyrighted by the contributors
  * recorded in the version of the history of the file, available from
  * its original location http://git.example.com/X/filename.c
  *
  * SPDX-License-Identifier: BSD-2-Clause
  * License-Filename: LICENSES / BSD-2-Clause_Charlie.txt
  * /
```

To ensure software compliance, these identifiers enable to generate automatically inventories of licenses in the form of "Bill of Material".

The complete list of SPDX identifiers is available at this address: [https://spdx.org/licenses/](https://spdx.org/licenses/)

## Traceability of development (DCO)

It is recommended to propose to contributors to sign a  _Developer's Certificate of Origin_. It allows her to attest that her contribution is genuine, respectful of previous works and that she accepts futur use for it under the project's license. A French translation is made available [DCO-Fr.txt](https://github.com/DISIC/politique-de-contribution-open-source/blob/master/DCO-fr.txt) and the english version is readble [here](https://developercertificate.org/).

In order to accept the DCO, the contributor only needs to sign off her commits with the command:

> `git commit --signoff` (or `git commit -s`)

A DCO procedure should preferrably be set at the beginning of the project and it should be clearly stated in the  `CONTRIBUTING` file of the repository.

## Development practices

Best development practices also apply in the context of open development, and in particular those related to the normative documents enforced within the administration:

* [General reference of interoperability](http://references.modernisation.gouv.fr/interoperabilite)
* [General accessibility reference framework for administrations](http://references.modernisation.gouv.fr/rgaa-accessibilite/)
* [General Security Reference](https://www.ssi.gouv.fr/administration/reglementation/numerique-confidence/the-referentiel-general-de-securite-rgs/)

Opening the code also amplifies the importance of some of these best practices:

* **Legal compliance** in the use of third-party libraries. The vast majority of current developments are based on third-party open source libraries, hence it is necessary to ensure the compatibility with their respective licenses and comply with their obligations.
* **Modularization of developments** to maximize code reuse but also to isolate any sources of error
* **Respect of a unique coding guideline** per project.
* **Documentation**, inside the code (comments and messages of * commit *) and outside the code (see below).

## Documentation good practices

The recommendations below are not mandatory rules but define a goal.  The quality of an open source project is closely related to the quality of its documentation, paying attention to this list is heavily recommended.

- The documentation is published under [**Licence Ouverte 2.0**][LO link].
- It is in sync with the software.
- It proposes a user manuel and a developer manual.
- It is available online (as a website) and offline (as a PFD document).
- It is written in proper french and/or proper english.
- It meets several expectations (FAQ, tutorials, reference manual, etc.)
- It contains zero or very few cultural or contextual references which may become obscure to future users.

## Security

### Identified interlocutor

It is recommended to identify a person in charge of the security of the project that will ensure compliance with best practices implemented during development, and to treat potential security incidents. It is also better to use a dedicated e-mail address to deal with security incidents or intellectual property issues which would be discovered by a third party.
 
### Secure development

* Write code that follows recognized security practices and that does not make use of dangerous constructions in the language used
  * [SEI CERT Coding Standards](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards)
  * PHP The Right Way (http://eilgin.github.io/php-the-right-way/)
  * [Secure Coding Guidelines for Java SE](http://www.oracle.com/technetwork/java/seccodeguide-139067.html)
  * [Importance of languages ​​for security](https://www.ssi.gouv.fr/agence/publication/mind-your-languages-new-article-on-the-importance-of-languages-for-security/ )
  * [Security and Java language](https://www.ssi.gouv.fr/javasec/)
  * [Security and functional languages](https://www.ssi.gouv.fr/lafosec/)

* Eliminate all *debug* messages (by compilation conditional or through a run-time variable) and any unnecessary information for the user in error messages (e.g. Java / PHP / Python call trace) when going into production

* Eliminate all dead code (*i.e.* code not called / no achievable) as it could be confusing and / or think that it is still functional and tested; this code, no maintained, could be wrongly reinstated by a developer
 
* All external inputs (e.g. user) must be checked before use or storage, according to good safety practices and in function of their destination.
 
### Do not rely on security by obscurity

Obscurity is generally recognized as an insufficient practice, but in the case of a project with open code, this strategy is deprecated. It must therefore be replaced by other more robust strategies such as defense in depth.

### Secret / sensitive data, cryptography

* No secret items (such as a password or key cryptographic) should only be stored in the code or in the comments; use configuration files that are not versioned (*cf* `.gitignore`)

* No secret element should be written by the program in clear in a file (including including a log file) or in a database, always prefer a hashed version with a state of the art hash function (*i.e* salt for each entry)
  * [General Security Reference System - Annex B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)
* No secret element must transit in clear on the network
* Do not implement a cryptographic mechanism yourself but use recognized libraries using parameters and robust cryptographic suites
  * [Security Recommendations for TLS](https://www.ssi.gouv.fr/nt-tls/)
  * [General Security Reference System - Annex B3](https://www.ssi.gouv.fr/uploads/2014/11/RGS_v-2-0_B3.pdf)


### Development tools and dependencies

* Use software and libraries where appropriate third parties maintained and up-to-date security patches; prefer libraries (re) known, and the simplest possible

* Use the code analysis services offered by the platform and systematically process problems brought up before integration

* Only push *commits* of code that compile, are tested, and functional, accompanied by corresponding unit tests; some platforms offer the opportunity to replay automatically the unit tests of a project to ensure the non-regression (e.g. [Travis](https://docs.travis-ci.com/), [Homu](https://github.com/servo/homu))

* Create a *tag* (e.g. v2.0.1) for each version (e.g. 2.0.1), and
sign it cryptographically (see [GPG signature
verification](https://github.com/blog/2144-gpg-signature-verification))

* Respect the recommendations and good safety practices issued by the ANSSI applicable to the project
   * [Good practices of ANSSI](https://www.ssi.gouv.fr/administration/bonnes-pratiques/)
   * [ANSSI / DINUM agile methodology security guide](https://www.ssi.gouv.fr/uploads/2017/07/guide-securite-agile_v0.42_anssi_dinsic.pdf)

## Tools

The contribution policy is not intended to offer specific tools. However specifically for managing open code, you can find the referenced tools on [https://www.linuxfoundation.org/tools-managing-open-source-programs/](https://www.linuxfoundation.org/tools-managing-open-source-programs/#1) useful.
