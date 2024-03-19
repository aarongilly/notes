---
created: 2023-08-11
aliases: 
tags:
  - data
---
**A fact table linked to many dimension tables that are normalized out to further sub-dimension tables.**

A snowflake schema is more normalized than a [[Star Schema]]. The dimension tables would link out to other sub-dimension tables via foreign keys rather than duplicate data. 

![[IMG_9715.png]]

****
### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Snowflake_schema)

### Related
- [[Facts vs Dimensions]]
- [[Star Schema]]