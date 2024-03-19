---
created: 2023-07-08
aliases: 
tags:
  - data
---
**A primary key that serves no other purpose.**

In the case a relational database table contains no single "best" [[Primary Key]] (or even no single *possible* Primary Key), a new field is added whose only purpose is to uniquely identify a row. These fields are often named "ID" or something to that effect. Fields whose only purpose in a table is to allow each row to be uniquely identified are called "Surrogate Keys".

Surrogate keys are necessary to prevent a collisions stemming from coincidence. For example: you have a student ID because your name is Joshua Brown and there's another "Joshua Brown" in your class.

Surrogate keys may often just be more convenient. You could concoct a crazy combination of fields that could, in aggregate, be called a primary key... but it's just easier to add an "ID" column and call it good. 

## Examples

- Social Security Numbers
- Student # or Employee #
- Account numbers

****
### Source

### Sources

[Primary key](https://en.wikipedia.org/wiki/Primary_key)

### Related
- [[Primary Key]] 
- [[Relational Databases]]