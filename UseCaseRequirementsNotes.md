**UC6** _data annotation_ (Manual or automated process for annotation of column headers/fields and streams. Could be done in real- or near-real time when the data are generated and subsequently transformed or in delayed mode.):

- Notes: 
	- manual and automated process may have differing requirements
	- m/a notation for requirement — x/x both required, x/ required for manual, /x required for automated
	
- Requires concepts that have persistent resolvable URIs
	- not required to perform action, but highly desirable, esp for subsequent data discovery
- Requires terminologies based on simple atomic terms
	- not absolutely required, but the more atomic the structure, the better the ability to annotate accurately, so highly recommended
- ADDED - Requires (agreement of) top-level, domain-independent categorization scheme/ontology
	- not required
- Requires that the relationships be trusted
	- not required
- Requires terminologies with coarse/fine granularity
	- not required, but highly desirable
	- the finer the granularity, the better the annotation capability
- Requires a long-term commitment governance setup
	- not required/required - manual annotation is done once; automated annotation is based on some kind of algorithmic approach that will need to be updated/maintained over time
- Requires an active community supporting the terminology
	- required if new terminology needs to be introduced for successful annotation
- Requires reliable technical infrastructure
	- required for automated annotation
- Requires input from domain experts
	- required for manual annotation
- Requires that the terminology be part of federated community specific and/or cross-domain portals
	- not sure
- Requires that the terminology supports multilingual terms
	- ideal, but not necessary
- Requires multilingual editorial team or multilingual community effort
	- ideal, but not necessary
- Requires terminologies published as linked data capabilities
	- very helpful, but not required
- Requires the terminology to use a common minimum metadata schema to describe semantic artefacts and their content
	- very helpful, possibly required (?)
- Requires mappings between terminologies
	- not required


**UC9** _keyword semantic data search_ (data discovery based on keywords that come from a controlled vocabulary):

- Notes: 
	- keyword semantic data search is greatly aided by the inclusion of synonyms (skos:altLabel)
	- main I’ve had with this kind of system is NASA’s GCMD Keywords
	
- Requires concepts that have persistent resolvable URIs
	- not required
- Requires terminologies based on simple atomic terms
	- not required, but the more atomic the structure, the better the semantic search results
- ADDED - Requires agreement of top-level, domain-independent categorization scheme/ontology
	- not required
- Requires that the relationships be trusted
	- not required
- Requires terminologies with coarse/fine granularity
	- not required
	- the finer the granularity, the better the search results
- Requires a long-term commitment governance setup
	- required in the maintenance of the controlled vocabulary
	- the way the CV is populated directly affects semantic search capabilities
- Requires an active community supporting the terminology
	- think so, but not sure
	- community can aid in providing alternate labels/synonyms
- Requires reliable technical infrastructure
	- yes (?)
- Requires input from domain experts
	- required in the maintenance of the controlled vocabulary
- Requires that the terminology be part of federated community specific and/or cross-domain portals
	- don’t think so
- Requires that the terminology supports multilingual terms
	- ideal, but not necessary
- Requires multilingual editorial team or multilingual community effort
	- ideal, but not necessary
- Requires terminologies published as linked data capabilities
	- very helpful, but not required
- Requires the terminology to use a common minimum metadata schema to describe semantic artefacts and their content
	- very helpful, possibly required (?)
- Requires mappings between terminologies
	- not required


**UC13** _data model alignment_ (harmonize different data models):

- Notes: 
	- two types of data model alignment methodologies 
		- pre-determined
		- on-the-fly/automated
	
- Requires concepts that have persistent resolvable URIs
	- ideally would have persistent URIs, but it is not necessary
- Requires terminologies based on simple atomic terms
	- yes, the more atomic the terms, the easier it is to create exact match alignments
	- however, atomization requires selecting a system of top-level, domain-independent disjoint categories; differing top-level categorizations among data models may impede successful alignment
	- therefore, this implicitly also requires agreement of top-level ontology
- ADDED - Requires agreement of top-level, domain-independent categorization scheme/ontology
	- required
- Requires that the relationships be trusted
	- yes
- Requires terminologies with coarse/fine granularity
	- requires the aligned terminologies to have the same level of granularity
- Requires a long-term commitment governance setup
	- not sure
	- may be necessary if aligned data models evolve independently
- Requires an active community supporting the terminology
	- don’t think so
- Requires reliable technical infrastructure
	- yes, especially if automated alignment is involved
- Requires input from domain experts
	- yes, alignment needs to be verified
- Requires that the terminology be part of federated community specific and/or cross-domain portals
	- think so
- Requires that the terminology supports multilingual terms
	- ideal, but not necessary
- Requires multilingual editorial team or multilingual community effort
	- ideal, but not necessary
- Requires terminologies published as linked data capabilities
	- very helpful, especially if domain expert input not available, but not required
- Requires the terminology to use a common minimum metadata schema to describe semantic artefacts and their content
	- very helpful, possibly required (?)
- Requires mappings between terminologies
	- if available, these can make alignment more straightforward, but not required
