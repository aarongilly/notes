---
created: 2023-12-08
aliases: 
tags:
  - data
  - systemdesign
  - modeling
summary: Tooling that ensures references between entities don't become outdated, dangling, or stale.
---
Referential Integrity refers to the consistency in associations between components in a system that are linked "by reference". Basically it's to do with whether or not data are dynamically linked, or hard-coded. Referential Integrity is also why [[TypeScript]] exists. Type-checking *enforces* referential integrity, and it's why the tooling of TypeScript helps so much more than standard [[JavaScript]] (not counting the benefits reaped through the usage of [[JSDoc]] with VSCode's tooling).

Referential Integrity is **always** a good thing. [[What is a System|System]]s that enforce RI are more durable, more adaptable, and allow for better agility in response to needed changes.

****
### Source
- 

### Related
- [[Entity-Relationship Modeling Standards]]
- [[Modeling Purposes]]