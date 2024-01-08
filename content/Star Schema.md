---
aliases: 
tags: [data]
---
**One fact table to many independent (but self contained) dimension tables**

A star schema is a less-normalized iteration of the [[Snowflake Schema]]. It is where a single fact table relates out to many dimension tables, but those dimension tables are not denormalized and do not _themselves_ branch out into additional sub-dimension tables.

![[IMG_9714.png]]

This is apparently the most common type of [[Data Warehouse]] schema used in industry.

---
### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Star_schema)

### Related
- [[Data Warehouse]]
- [[Snowflake Schema]]
- [[Facts vs Dimensions]]
 