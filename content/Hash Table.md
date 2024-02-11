---
created: 2023-07-08
aliases: 
tags:
  - data
  - coding
---
**A data structure enabling very fast retrieval of data by loading values into slots based on a hash function**

Hash Tables are data structures holding values in an array in a position according to their value (or key, etc) calculates through a hashing function. This allows you to look up values from the hashing table in constant time - you don't have to look index-by-index to find the element you're searching for. You can apply the a hashing function then go look there. 

There is no such thing as a universal perfect hashing function. Hashing collisions occur when two separate values to store result in the same hashing function output. This causes the 2nd value to have to find a new location to live in accordance with some sort of collision handling strategy. 

---

### Source
- [[Wikipedia]]

### Related
- [[Types of Non-relational Databases]] 
- [[Data Topics]] 
- [[Relational Databases]]