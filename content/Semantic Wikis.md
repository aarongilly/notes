---
created: 2023-07-08
aliases: 
tags:
  - modeling
  - notetaking
---
**A wiki with structured entries and meaningful links between them.**

A semantic wiki is a wiki in which both the entries and the relationships between them can be “typed” with names and associated metadata. A semantic wiki differs from a regular wiki because it allows for implicit knowledge inference and for robust queries using languages like you'd find in a [[Graph Database]]. Semantic wikis can be considered a form of [[Ontology]] software.

Semantic Wikis would have [[Entity Definition]]s, and definitions of [[Entity Relationship Categories]]. The relationships *between the relationships* would **also** be made explicit. You'd probably be best served having a type of entity titled "relationship", whose class could be used as edges in the graph. If the relationship categories themselves weren't pertinent to the knowledge graph, then you could use a [[URI]] scheme and reference external repos for the [[Ontology]]. This is what the 4th term in [[Resource Description Framework|RDF]] quad stores effectively does, I think. Or maybe not. Regardless it seems like it might be a good practice to **include the relationships themselves as entities** in the wiki. For that matter, you'd probably want constraints. Actually designing a Semantic Wiki might be awesome.

Example pseudo wiki code:
```yaml
Entity_Name: Living Person
Definition: A human being who was born at some point.
Properties: 
	Name: string
	Birthday: Date

Entity_Name: Dead Person
Extends: [Living Person]
Properties:
	Death_Date: Date

Relationship_Name: Family
Label_From: Is family with
Label_To: Is family with
From_Types: [Living Person, Dead Person]
To_Types: [Living Person, Dead Person]

Relationship_Name: Parent
Label_From: Has Child
Label_To: Has Parent
From_Types: [Living Person, Dead Person]
To_Types: [Living Person, Dead Person]
Subtypes: [Family]
```
	
****
### Source

### Related
- [[Types of Non-relational Databases]] 
- [[Ontology]] 
- [[Resource Description Framework]]