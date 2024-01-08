---
aliases: 
tags:
  - data
---
**The identifier of a row in a table. May be a combination of fields or a single field.**

In [[Relational Databases]], each row much be able to be unique identified. This is done by setting a rule (either informally, in the case of Excel Workbooks, or formally, in the case of managed proper databases) that states "no two rows may exist that share the same value in this field (or combination of fields), AND no row exists for which this field contains no value".

If a Primary Key is derived from a combination of multiple attributes, then it is referred to as a [[Composite Key]] .  

A table may have many [[Candidate Key]]s, but only one such key will be crowned "primary". All other candidate keys are referred to as "Alternate Keys".  All fields contained in sets of candidate keys are called "[[Prime Attributes]]". 

Primary Keys which were **only** added to unique identify rows are called [[Surrogate Keys]].

Attributes in a table that are Primary keys in other table(s) are called [[Foreign Key]]s.

---

### Source

### Source

[Primary key](https://en.wikipedia.org/wiki/Primary_key)

### Related
- [[Candidate Key]] 
- [[Relational Databases]] 
- [[Surrogate Keys]] 
- [[Foreign Key]] 
- [[SQL]]