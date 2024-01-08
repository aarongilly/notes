---
aliases: 
tags:
  - coding
  - modeling
  - data
---
**Key-Value stores, document databases, graphs, and other NoSQL database types.**

## Key-Value Store

Literally just a big collection of key-value pairs. Keys appear just once per database.

## Document Store

Stores of [[JSON]], [[YAML]], or [[XML]]. These are highly flexible.

## Graph

Sets of edges and nodes. Allowing for highly-linked data. In graphs, the relationships between nodes are themselves capable of holding information. Graphs allow for semantic queries, where you can specify things like "show me all the liked posts by friends of my friends" naturally.

## Triple Store

Triplestores store triples. These store semantic triples, which are datasets of the form "Subject-Predicate-Object", like "Man has ball", or "Aaron married Melissa". 

### Named Graph

Named graphs are extended Triplestores, with a fourth dimension specifying their context. They are of the basic form "Subject-Predicate-Object-Context". 

---

### Source

[NoSQL - Wikipedia](https://en.wikipedia.org/wiki/NoSQL)

### Related
- [[Relational Databases]] 
- [[Non-Relational Databases]]