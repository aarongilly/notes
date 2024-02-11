---
created: 2023-07-08
aliases: 
tags:
  - data
---
**Quick overview 1NF-3NF**

Data normalization exists in multiple levels, according to multiple rules. Normalization reduces data redundancy and increases data integrity. Informally, the cutoff for "well-normalized" is between 3NF and 4NF. Eventually, 6th Normal Form is what you'd call a whole host of Key-Value pairs, where the key is a [[Primary Key]] (this is known as a "Columnar data store").

For well-Normalized data... put simply:

> Every non-key attribute
depends on the key (1st normal form)
the whole key (2nd normal form)
and nothing but the key (3rd normal form)
- Colorado State Paper
> 

Unnormalized Data

- anything goes

First Normal Form (1NF)

- Cells contain only one value

Second Normal Form (2NF)

- Cells contain only one value
- All non-Prime fields are functionally dependent on the whole primary key

Third Normal Form (3NF)

- Cells contain only one value
- All non-Prime fields are functionally depending on the whole primary key
- All non-Prime fields are independent of each other

---

### Source

### Source

[Relational Database Schema Design Overview](https://medium.com/@kimtnguyen/relational-database-schema-design-overview-70e447ff66f9)

[Database normalization](https://en.wikipedia.org/wiki/Database_normalization)

[](https://www.cs.colostate.edu/~cs430dl/yr2020su/more_examples/Ch8/Identifying%20Normal%20Forms.pdf)

### Related
- [[Relational Databases]] 
- [[Primary Key]] 
- [[Prime Attributes]] 
- [[Superkey]] 
- [[Composite Key]]