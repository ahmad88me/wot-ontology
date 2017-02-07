# vicinity-ontology-wot summary
Repository for collaborative edition of the VICINITY ontology module for the Web Of Things domain. This ontology is being developed within the context of the [VICINITY H2020 project] (http://vicinity2020.eu/).

To include issues for this domain (that is, things you need this ontology to represent or improve): https://github.com/mariapoveda/vicinity-ontology-wot/issues

The ontology latest release is published at: http://iot.linkeddata.es/def/wot/ (draft)

Relevant links:

- [WoT interest group current practices] (http://w3c.github.io/wot/current-practices/wot-practices.html)
- [WoT demos] (https://www.w3.org/WoT/demos/td2ttl/)

# How We Work
This document provides a brief overview of the process for developing the [WOT ontology](http://iot.linkeddata.es/def/wot/). It contains a minimal amount of technical detail sufficient to explain our approach to collaborative ontology development.

## Overview 

- VICINITY provides a core ontology for describing the core information to be used in VICINITY ecosystem. This core ontology, which relies in more general modules or cross-domains ontologies (e.g., time, space, web things, etc.), might be extended for more specific domains and applications (e.g., health, buildings, transport, etc.)
- Each domain is going to be stored in a GitHub repository. This repository hosts the [WOT ontology](http://iot.linkeddata.es/def/wot/).
- Improvements and issues for each domain are discussed in the repository's GitHub issue tracker ([issues for the WoT ontology] (https://github.com/mariapoveda/vicinity-ontology-wot/issues))
- The requirements of each domains are stored in a Google Spreadsheet ([WoT ontology requirements] (https://docs.google.com/spreadsheets/d/1_VcoGD5Qq6iKr8-XNGJGsOo475aiZsnKf0i01awdZkc/edit#gid=0)). When there is a release version a domain, the spreadsheet is automatically converted to HTML and commited to the repository.
- The ontology developers have to evaluate the ontology and generate its documentation before publishing it.
- The releases versions of the domains are published in the site.
- OnToology will generate the documentation and the evaluation of the ontology. 
- The list of VINICTY ontologies are listed in: http://vicinity.iot.linkeddata.es

## Structure of the GitHub repository

The sytem selected to store the ontology is GitHub. Each module in VICINITY ontology will be stored in a repository. We will also have an aggregator repository which integrates all the modules and submodules of VICINITY Ontology (not available yet). Each repository will include:

- An evaluation folder where the evaluation reports of the ontology are stored.

- A documentation folder where the documentation reports of the ontology are stored, including the requirements and the description of the ontology.

## GitHub Flow

For developing an ontology using GitHub the developers can follow the [GitHub good practices guides](https://guides.github.com/). Basically, the central repository holds a main branch called master where the source code reflects the production-ready state.To work on something new, the ontology developers have to create a descriptively named branch off the master, so that the rest of the developers can see what is being worked on. Once the branch is created, the developers add changes to the ontology and commit them. Each commit has to be associated with a commit message, which is a description explaining why a particular change was made, so that the developers can roll back changes if a bug is found. After adding commits, the ontology developers have to open a pull request to discuss the modifications done to the ontology. If everyone agree, the pull request is accepted and the changes are merged to the *master* branch.

## Development process

Once the ontology is implemented (for this step you can use an ontology editor like [Protégé](http://protege.stanford.edu/)), it has to be evaluated and documented before its publication.

### Ontology Evaluation
The ontology has to be evaluated according to syntactic, model and semantic errors. OnToology will evaluate the ontology using [OOPS! OntOlogy Pitfall Scanner!](http://oops.linkeddata.es/) and generate an evaluation report every time there is a push in the repository (if selected in OnToology config file). The ontology developers also have to guarantee that the ontology meets all the requirements identified. 

### Ontology Documentation

OnToology will generate the documentation using [Widoco](https://github.com/dgarijo/Widoco) every time there is a push in the repository. This documentation includes an HTML description of the ontology which describes the classes, properties and data properties of the ontology, and the license URI and title being used. The ontology development team in collaboration with the domain experts can complete this HTML documentation. OnToology will also generate the diagrams using [AR2DTool](https://github.com/idafensp/ar2dtool. It will generate two kinds of diagrams:

- Class diagram
- Taxonomy diagram

### Ontology Publication

Releases are published in the official site by the project webmaster, so the ontology and its documentation will be accessible to all the users. The site will publish additionally for each ontology the repositiory where is stored, its issue tracker and the requirements associated to each ontology.

### Ontology Maintenance
If the ontology developers or domain experts want to update or add new requirements to the ontology they will need to create a new issue [in this GitHub issue tracker for the WoT ontology](https://github.com/mariapoveda/vicinity-ontology-wot/issues) (for other domains see the [VICINITY ontology index](http://vicinity.iot.linkeddata.es)). This issue will let the developers to start a discussion and accept or regret the modifications. GitHub also provide a good practices guide for [creating issues](https://guides.github.com/features/issues/). 
