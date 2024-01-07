---
created: 2023-08-11T17:32-05:00
updated: 2024-01-01T23:28-06:00
tags:
  - data
---
**A fact table linked to many dimension tables that are normalized out to further sub-dimension tables.**

A snowflake schema is more normalized than a [[Star Schema]]. The dimension tables would link out to other sub-dimension tables via foreign keys rather than duplicate data. 

![[IMG_9715.png]]

---
### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Snowflake_schema)

### Related
- [[Facts vs Dimensions]]
- [[Star Schema]]