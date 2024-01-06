---
tags:
- coding
- modeling
- data
---
**Universally Unique Identifier - a 128-bit identifier**

UUID stands for "Universally Unique Identifier". The idea is that it's a [[Surrogate Keys]] that function for *any* element of *any* table, resource, system, or whatever. It's **universal**.

It was developed my Microsoft, and is typically 128-bits. They are supported by Microsoft SQL Server, MySQL, PostgreSQL, MongoDB, and others.

### Format

There are 5 Versions of UUIDs. Some are random. Some are time-indexed. They generally are broken into 5 groups of **hexadecimal** characters, delimited by hyphens. Like so:

`123e4567-e89b-12d3-a456-426614174000`

What each of those hyphen-delimited groups *means* depends on the version of the UUID. 

---

### Source
- [Universally unique identifier - Wikipedia](https://en.wikipedia.org/wiki/Universally_unique_identifier)

### Related Notes
- [[SysML]] 
- [[Primary Key]] 
- [[Surrogate Keys]]
- [[UUIDs in the Wild]]