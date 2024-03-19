---
created: 2023-07-08
aliases: 
tags:
  - modeling
  - data
---
**Facts are the money spent, Dimensions are where and when.**

Facts and dimensions both look like columns in a table, and they are, but they carry a different purpose. 

Facts are the raw, usually numeric data. These are the things that retain meaning when you roll them up in a summary.

Dimensions are the data associated with the facts that give them meaning. These are things like times, locations, people, or object attributes (e.g. Project Status). These often (always?) come from [[Master Data]].

Typically there are many fewer rows in dimensions than their would be facts. 

## Examples
- Mint Financial Data
    - Facts - transaction amount
    - Dimensions - vendor, account, date
- Phone
    - Facts - number of calls made, data used
    - Dimensions - phone numbers called, dates, account number

****
### Source 
- [Wikipedia](https://en.wikipedia.org/wiki/Data_warehouse)

### Related
- [[Star Schema]]