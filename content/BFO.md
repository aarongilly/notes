---
aliases: 
tags:
  - learning
  - modeling
  - data
---
**The Basic Formal Ontology [[Ontology]] **

BFO is the ‘Basic Formal [[Ontology]] ’, which is an upper-level (domain-independent) ontology for scaffolding out lower-level (domain-specific) ontologies. There are multiple domain-specific ontologies that are extensions of the BFO (e.g. - the [information artifact ontology](https://github.com/information-artifact-ontology/IAO)). The BFO is documented in the spec & the OWL language.

![[IMG_0964.jpeg.jpeg]]

It's a hierarchy. The top-level split is a breakdown into a thing that exist and endures (a “[[Continuant]]“) and a thing that *happens* (an “Occurent”). This is basically the “Objects” and “Processes” from [[OPM]].

### Entities
An entity is anything that can exist. It can be divided into ******************instances****************** (my heart, your heart), and ********************universals******************** (’*heart*’ in general). The BFO spec uses italics when referencing to universals.

### Is_A Overloading
The BFO uses a much more strict and narrow definition of “Is_A” than our standard usage in English might allow. In BFO vernacular, “X Is_A Y” strictly means X is a subtype of Y. Not X is an instance of Y.

### Determinables and Determinates
The BFO calls numeric measurements “Determinates” and their ancestors “Determinables”. So, “5lbs weight” is a determinate and “mass” is the determinable.

### Notes Note.
There’s much more I could write about, but then I’d have to read it. This is not a universal truth, it’s an instance of how a group of folks decided to carve up describing the world.

---

### Source
- [[Basic Formal Ontology 2 0 Spec]]

### Related
- [[OPM]] 
- [[Ontology]]