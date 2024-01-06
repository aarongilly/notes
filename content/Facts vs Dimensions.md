---
tags:
- modeling
- data
---
**Facts are the money spent, Dimensions are where and when.**

Facts and dimensions both look like columns in a table, and they are, but they carry a different purpose. 

Facts are the raw, usually numeric data. 

Dimensions are the data associated with the facts that give them meaning. These are things like times, locations, people, or object attributes (e.g. Project Status).

Typically there are many fewer rows in dimensions than their would be facts. 

## Examples

- Mint Financial Data
    - Facts - transaction amount
    - Dimensions - vendor, account, date
- Phone
    - Facts - number of calls made, data used
    - Dimensions - phone numbers called, dates, account number

---



### Source
- [Wikipedia](https://en.wikipedia.org/wiki/Data_warehouse)

### Related Notes
- [[Star Schema]]