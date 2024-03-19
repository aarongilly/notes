---
created: 2024-01-28
tags: [data, todo]
aliases:
---
There is no "global" set of data types. There are a few candidates that are (nearly) globally implemented across [[Non-Relational Databases]], [[Relational Databases]], and programming languages - but it's always dependent on the specific [[Ontology, Semantics, and Syntax|syntax and semantics]] of the language. 

## Type Table
This is a hilariously incomplete table. I didn't want to do a thousand rows. 

| Type | SQLite | JavaScript | Python | Postgres | CSV/JSON |
| ---- | ---- | ---- | ---- | ---- | ---- |
| int | ✅ |  |  |  |  |
| bool |  |  |  |  |  |
| null | ✅ |  |  |  |  |
| blob | ✅ |  |  |  |  |
| real | ✅ |  |  |  |  |
| text/string/str | ✅ |  |  |  |  |
| char |  |  |  |  |  |
| enum |  |  |  |  |  |
| map |  |  |  |  |  |

**PostgreSQL** has a [boatload](https://www.postgresql.org/docs/current/datatype.html) of supported types. 

****
### Source
- 

### Related
- [[Data Warehouse]]
- [[Data Serialization]]
- [[Data Serialization Methods]]