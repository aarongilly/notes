---
created: 2023-07-08
aliases: 
tags:
  - data
  - modeling
  - coding
---
**Composition: Children can’t exist without parent. Aggregation: Children can exist separately from parent.**

Aggregation and Composition are very similar. The difference is whether or not the children can possibly exist without the parent. Composition implies ****************************************************************************************when a parent is deleted, the children are also deleted****************************************************************************************. Aggregation has no such implication. 

They still seem like they are used almost interchangeably in practice. From the source:

![Untitled](Untitled%2037.png)

Interestingly - the UML 2.5 Specification doesn’t even define ‘Aggregation’. Like it’s not in there at all when you Ctrl+f ‘aggregation’.

****
### Source

### Source

[UML Association vs Aggregation vs Composition](https://www.visual-paradigm.com/guide/uml-unified-modeling-language/uml-aggregation-vs-composition/)

### Related
- [[Entity Relationship Categories]] 
- [[UML]]