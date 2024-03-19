---
created: 2023-07-08
aliases: 
tags:
  - data
---
**A set of fields combinations which could be considered for Primary Key.**

In [[Relational Databases]], a "Candidate Key" is basically a (set of) field(s) inside a table that ***could*** unique identify one row (a.k.a. "[[Tuple]]")... but isn't *necessarily* being used to do that, functionally. Any given table may have multiple Candidate Keys, but only one of them may be chosen as the "[[Primary Key]]". 

Candidate Keys reveal the possible ways in which a DBA could positively identify a single Tuple. One such way will be chosen & blessed as the "Primary Key". Other sets that would also function are all considered "Alternate Keys". Candidate Keys are just the Primary Key and all sets of possible Alternate Keys.

****
### Source

[Candidate key](https://en.wikipedia.org/wiki/Candidate_key)

### Related
- [[Primary Key]] 
- [[Relational Databases]]