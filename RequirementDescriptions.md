# Requirement Descriptions

This document is intended to find canonical descriptions for the requirements listed in [the respective Google Sheets](https://docs.google.com/spreadsheets/d/1nhVm98cBXCLJ5Ni6X3TYHAcXfOVY7eWHO7Q8cBmjqLI/edit#gid=665493837).

A description should …
*   make it easy to understand the respective requirement and make an assessment in the use cases.
*   clearly distinguish the requirement from other similar requirements.

Constraint: If we ask for something to be included (like multilingual terms or mappings) it is always implied that this is reliable (in all senses like persistent, high quality, …).

The reference to the Fair Semantic Criteria is taken from the DRAFT version v1.0 of Le Franc, Y., Parland-von Essen, J., Bonino, L., Lehväslaiho, H., Coen, G., & Staiger, C. (2020). D2.2 FAIR Semantics: First recommendations - DRAFT. [https://doi.org/10.5281/ZENODO.3707985](https://doi.org/10.5281/ZENODO.3707985)


## Requires concepts that have persistent resolvable Uniform Resource Identifier (URI)s

**Description**: 
The use case requires that each term/concept should be assigned a globally unique and persistent identifier. The identifiers are maintained and governed such that they remain stable and resolvable for the long term. Example of a concept identified with persistent URI (not limited to) is [http://purl.bioontology.org/ontology/MEDDRA/10029205](http://purl.bioontology.org/ontology/MEDDRA/10029205); [http://vocab.nerc.ac.uk/collection/P02/current/BCAH/](http://vocab.nerc.ac.uk/collection/P02/current/BCAH/).

**Relates to:**
* Fair Semantics Criteria: P-Rec. 1: Use Globally Unique, Persistent and Resolvable Identifier for Semantic Artefacts, their content and their versions


## Requires the terminology be hosted by a trustworthy semantic repository

**Description:**
The use case requires that terminologies be hosted and accessible through  one or multiple synchronised dedicated infrastructures (repository, server) enabling users to retrieve curated concepts in a reliable and automated way. Criteria for trustworthiness to be defined.
The CoreTrustSeal Trustworthy Data Repositories Requirements (10.5281/zenodo.3638211) describe the characteristics of trustworthy repositories and define 16 requirements.

**Examples:** 
* NERC Vocabulary Server
* Research Vocabularies Australia
* OBO Foundry
* EcoPortal.

**Relates to:**
 * Fair Semantics Criteria P-Rec. 4: Publish the Semantic Artefact and its content in a semantic repository

## Requires terminologies based on simple atomic terms (e.g. used to make more complex compound terms)

**Description:** 

The use case requires standalone terms that can be given meaningful definitions in their own right and can be combined (following the semantic model of the terminology) to create new, compound terms.

Examples of simple atomic terms are:
* water body (e.g. **[http://purl.obolibrary.org/obo/ENVO_00000063](http://purl.obolibrary.org/obo/ENVO_00000063)**)
* Flower (e.g. **[http://purl.obolibrary.org/obo/PO_0009046](http://purl.obolibrary.org/obo/PO_0009046)**)
* Color (e.g. **[http://purl.obolibrary.org/obo/PATO_0000014](http://purl.obolibrary.org/obo/PATO_0000014)**)
* temperature (e.g. [http://qudt.org/vocab/quantitykind/Temperature](http://qudt.org/vocab/quantitykind/Temperature)) , 
* ammonium ([https://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI:28938](https://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI:28938)), 
* grain size ([http://vocab.nerc.ac.uk/collection/S06/current/S0600192/](http://vocab.nerc.ac.uk/collection/S06/current/S0600192/))
* etc.

Examples of compound or composite terms:

* Flower + color: **[http://purl.obolibrary.org/obo/TO_0000537](http://purl.obolibrary.org/obo/TO_0000537)**
* Grain-size + other terms: [http://vocab.nerc.ac.uk/collection/P01/current/MDGSPSXX/](http://vocab.nerc.ac.uk/collection/P01/current/MDGSPSXX/)
* etc.


## Requires (agreement of) top-level, domain-independent schema or ontology

**Description:** 
The use case requires that at least two or more terminologies have been successfully aligned through a domain independent resource which is sufficiently generic and establishes semantic equivalences between concepts.

**Relates to:**
* Fair Semantics Criteria P-Rec. 10: Use a Foundational Ontology to align semantic artefacts


## Requires that the terminology includes semantic relations between its concepts 

**Description:**

The use case requires that there should be at least a relation between a term and another term within the same terminology. 

Examples of relations are synonyms, part-of, broader and narrower (all structural/SKOS relationships) - do we need to consider others, semantically richer relationships?


## Requires mappings between terminologies

**Description:** 

The use case requires that mapping to external resources be supported i.e. terms in a terminology are aligned to corresponding terms in another terminology. Do we also need to specify that the alignments are or need to be curated? 

**Examples:**
* Bioportal ([http://bioportal.bioontology.org/mappings](http://bioportal.bioontology.org/mappings))


## Requires that the provenance and status metadata of mappings between concepts  be accessible.

**Description:**

The use case requires that there should be an easily accessible record of the authority responsible for creating the mapping, (for example, was the mapping created by human or machine?) and of its status (e.g. Hhas it been checked or certified in any way?). (N.B. I think this is the same as requirement “Requires metadata indicating mapping type (automated/manual) and validity (i.e. status)”, page 5)

There is a proposed Ontology Mapping Language we can point to.

**Relates to:**
* Fair Semantics Criteria P-Rec. 13: Crosswalks, mappings and bridging between semantic artefacts should be documented, published, and curated


## Requires coarse-grained terminologiess for observable properties

**Description:** 

The use case requires human and machine-readable terms that identify observable properties at a fairly broad descriptive level (e.g. “organic compounds” or “nitrate in water” or “chlorophyll distribution”). These terminologies are ~~typically~~ often used at the top or mid-layer of concept hierarchies and contain enough information to enable, e.g., semantic data search. These broad concepts can be used to group more detailed concepts in finer-grained terminologies, in ontologies or thesauri (see next requirement below). Some terminologies have coarse granularity, some have fine granularity and some (e.g. CF standard names) contain a combination of both.

Example of coarse granularity observable property term: [http://vocab.nerc.ac.uk/collection/P02/current/NTRA/](http://vocab.nerc.ac.uk/collection/P02/current/NTRA/)


## Requires fine-grained terminologies for observable properties

**Description:** tbd

Examples of fine granularity observable property term: [http://vocab.nerc.ac.uk/collection/P01/current/NTRZKGD5/](http://vocab.nerc.ac.uk/collection/P01/current/NTRZKGD5/)


## Requires a long-term commitment to the terminology content governance

**Description:**
The use case requires a long-term commitment to maintaining a clear content governance structure so that the terminology remains relevant to the community it serves and continues to reflect current usage of scientific terms. Both terms and their definitions should be maintained and changes should be documented. Many terminologies have their own governance procedure which should be documented and published, e.g., http://cfconventions.org/standard_name_rules.html


## Requires a community-endorsed terminology

**Description**: tbd


## Requires the terminology to be discoverable (not just technically but also e.g. listed in relevant community portals or discoverable via search engines)

**Description:** The use case requires terminologies that can be discovered by machines and humans. For example, through a terminology search api ([https://www.itis.gov/web_service.html](https://www.itis.gov/web_service.html)) and  terminology portal/user interface (e.g., [https://www.itis.gov/](https://www.itis.gov/))  supported by a repository (e.g., Integrated Taxonomic Information System) or beyond the repository it is curated such as terminology aggregator (Bioportal).


**Comments:** FAIR F4 from the provider perspective but here it is from the User perspective

Terminology is findable through other portals, beyond the repository it is curated.


## Requires that the terminology provides multilingual terms

**Description:**

The use case requires terminologies that support and enable input of information in multiple languages. 

## Requires common, minimum metadata describing the terminology 

**Description:**

The use case requires terminologies that comply with a minimum (mandatory) set of community-agreed machine-readable metadata information about the terminology  infrastructure and its content. The common minimum metadata schema is expected to be derived from the FAIR semantics recommendation and from work like e.g. Ditta et al (MOD - ref needed) 

**Fair Semantics Criteria:** P-Rec. 3: Use a common minimum metadata schema to describe semantic artefacts and their content


## Requires definitions of the individual terms within a terminology

**Description:** The use case requires that concise descriptions (human readable text) of each of the terms in a terminology should be provided, and the descriptions should be easily accessible alongside the terms.

We should cite the papers about how to write a good ontology definition.


## Requires that any underlying model used by the terminology to be described and accessible

**Description:** 
The use case requires that the underlying data model be clearly described and accessible to machines and humans.

**Examples:**
* Data model of the terminology ‘XX’ is YY.


## Requires the provenance properties of individual terms to be documented in a standardized way.

**Description:** The use case requires that the history of a term and its development needs to be recorded along with the attribution for the editors doing the work. This can be accomplished using versioning in GitHub and ORCIDs for attribution. 

**Examples:**


## Requires examples of usage of the terminology to be available and documented

**Description:** The examples of the application of the terminology should be documented and accessible.


## Requires the terminology to be accessible programmatically. 

**Description:** tbd

The use case requires the terminology to be accessible via a programmatic interface such as a web service or access endpoint. 

**Examples:** 
* REST, SOAP, SPARQL endpoint, content negotiations, typed link


## Requires deprecated term status and deprecation policy

**Description:**
The use case requires that terms be labeled as deprecated or active and a clear deprecation policy (e.g. whether deprecated terms will remain referenceable in perpetuity, whether deprecated terms will reference non-deprecated terms that can be used as substitute, etc.)

**Examples:** 
* OBO Foundry has a policy we can start from


## Requires tools supporting annotation using the terminologies.

**Description:**

**Examples:**


## Requires tools validating the applied terms against the terminologies

**Description:**
The use case requires a tool to be able to validate applied terms or URIs said to come from the terminology.

**Examples:**


## Requires tooling for mapping

**Description:**
The user case requires a tool to align selected terminologies.

**Examples:**


## Requires a mean to manage alternative notations 

**Description:**
The use case requires a mechanism for annotating concepts with multiple alternative labels, including formal standardized names, common names, formulas, abbreviations or common misspellings. Examples: “carbon dioxide” and “CO2” are labels for the same concept; a terminology may choose to use SKOS (as an example) to assign one of these labels with `skos:prefLabel` and the other term with `skos:altLabel`.

**Examples:**

## Requires a collaborative terminology development policy.

**Description:**
The development of the terminology is not bound to a specific group of people, but is open to anybody interested. External contributors can align the terminology with the progress in the respective community and ensure the terminology’s accuracy over time. There should be additional gatekeepers to prevent vandalism and erroneous changes.

**Examples:**
